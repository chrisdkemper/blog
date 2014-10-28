---
layout: post
title:  "Date filtering in jQuery DataTables"
date:   2014-10-28 11:39:09
comments: true
categories: jQuery
---

On a recent project, I had to add date filtering to a jQuery DataTable instance, which isn't as easy as I'd hoped. The [documentation](http://datatables.net/plug-ins/filtering/) implies this is possible, but after looking it up, couldn't find anything helpful.

In this case, the data was supplied with an AJAX source (which was required given the amount of data), so instead of hooking into the column data and doing it on the front-end, I took advantage of `preXhr.dt`, which is used via the DataTable `on` method.

My DataTable object, ended up looking like this:

{% highlight js startinline %}
var to = $('#to');
var from = $('#from');
var table = $('#table')
    .on('preXhr.dt', function ( e, settings, data ) {
        data.from   = from.val();
        data.to     = to.val();
    })
    .DataTable({
        "order": [[ 1, "desc" ]],
        "sPaginationType": "full_numbers",
        "bSort" : false,
        "bFilter": false,
        "bProcessing": true,
        "bServerSide": true,
        "bDeferRender": true,
        "sAjaxSource": "/data",
        "sDom": 'ltipr',
        "columns": [
            { "data": "name" },
            { "data": "date" },
            { "data": "postcode" }
        ]
    });

table.draw();
{% endhighlight %}

This essentially takes the values from the `to` and `from` fields (jQuery date pickers) and passes them along with the other date, for every AJAX request. This means, you can check if these values exist, then filter on them accordingly before returning the table.

To get this all running, just add an `onSelect` callback to the datepicker, and you're all set

{% highlight js startinline %}
$(".date").datepicker({
    dateFormat: "dd/mm/yy",
    onSelect : function(date, inst) {
        table.draw();
    }
});
{% endhighlight %}

This way you can use you own names for the form, style the filter however you want, and choose how to treat the data. This can of course be used with any other filter, I just happened to use a date range.