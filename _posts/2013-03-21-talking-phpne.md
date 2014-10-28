---
layout: post
title:  "Talking at PHPNE"
date:   2013-03-21 11:39:09
comments: true
categories: misc speaking
---

On Tuesday, the 16th of April, I gave a talk at PHP North East, titled "Silex: From nothing, to an API". This was my first real talk, so it was really nerve wracking for me. Initially, I planned not to be the guy who wrote his presentation the night before, but due to certain things, that turned out to be what happened.

This lack of planning and rehearsal time really came to be a real problem for me, as during my actual talk I rushed through my slides, and missed out some key points. The Friday following my talk, I was also involved in a workshop on how to give better presentations, which, I wish had of been the Friday before my talk, but never mind.

After the course, and listening to myself during the talk, I've realised a number of issues with it. The following are things that I either learned, or did incorrectly during my talk.

You can see the slides for the talk on [slideshare](http://www.slideshare.net/chrisdkemper/silex-from-nothing-to-an-api) and the source code on [GitHub](https://github.com/chrisdkemper/PHPNE-Silex). Also, if you have any feedback on the talk, please let me know via [Twitter](http://twitter.com/chrisdkemper) (@chrisdkemper) or in the comments.

##1. Don't make assumptions

This was my first real problem, as it lead to a few issues during the talk. My first assumption, was that I thought everybody in the room would know about Composer, which after the talk, I learned wasn't the case. I don't believe in explaining every part of a presentation, because this can be very boring to the majority of spectators, and makes for a dull presentation. I could have however, put a slide in explaining what Composer was and its benefits. Within this slide I could have also mentioned Composers ability to autoload a users own libraries, which I used within the presentation, but never explained.

To make life easier for myself during the testing part of the part, I'd written some tests using the [Symfony Console Component](http://symfony.com/doc/2.0/components/console/introduction.html) but I then didn't fully explain this. I should have made a better point of mentioning that it wasn't part of Silex, and was a separate library. I also could have actually explained the benefits of this a lot more, as the library itself is awesome, and you should check it out.

##2. Slow the fuck down

After the course, and listening to myself during the presentation, I know now that I was talking through my slides WAY too fast. This is a vicious cycle, because as you talk faster, you go through more slides, and then realise you don't have many slides left, which makes you more nervous, so you talk faster, etc, etc. With being nervous I missed out explaining some of the key parts of the talk. First of all, I should actually explained how Silex works with its routes. The first example I used, is the one mentioned in the documentation on the Silex website is quite simple to someone who knows Silex, but not for someone who is unfamiliar with it. Below is that code sample:

{% highlight php startinline %}
$app->get('/hello/{name}', function($name) use($app) {
   	return 'Hello '.$app->escape($name);
});
{% endhighlight %}

Ideally, I should have mentioned that each route is added to the main application object, and that variables used in the url are passed through as arguments. You can also use the Request and Response objects as arguments too, if you require them within the route. Also, to make use of application helper functions and services, the application variable needs to passed into the route via use, otherwise it'll be unavailable within the route.

I also rushed through the usage of components within the application. I didn't elaborate very much on the use of DBAL within the talk. Although it was only a base usage, I could have still went into a little more detail about how it worked, but I blame my nerves.

##3. Plan Plan Plan
My lack of preparation time kicked me in the face here. For one, I mentioned some things that weren't technically correct. These were mainly down to the use of Silex in larger applications. Silex as a framework is perfectly capable of handling larger applications, but the issue with it comes with managing the routes, as this can get quite messy unless it's managed properly. You can get around this a little by using [Controller providers](http://silex.sensiolabs.org/doc/providers.html), which can make routes a lot more manageable for larger applications.

I also totally neglected to mention how easy it is to run tests within Silex, you can check that our [here](http://silex.sensiolabs.org/doc/testing.html).

##Summary
There were a few other improvements I could have made, but on the whole I'm still glad I gave the presentation. Although there were a lot of problems, I learned a lot from the experience, and, I know at least one person got something out of, which makes it all worth it! Hopefully I'll be able to do another talk in the future, and make a better job of this one.