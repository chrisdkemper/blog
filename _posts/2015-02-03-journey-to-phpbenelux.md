---
layout: post
title:  "A journey to #PHPBenelux"
date:   2015-02-03 12:25:09
comments: true
categories: php
summary: My experience at #PHPBenelux15
---

TL;DR I went to PHPBenelux, I learned a lot, it was awesome!

Not only was this my first PHPBenelux, it was also my first non-UK based conference, so this was a pretty big deal for me. We ([Anthony](http://twitter.com/AnthonySterling), [Peter](https://twitter.com/peterwardle) and I) arrived on Thursday night and headed to the main conference on Friday. Since we didn't have tutorials or anything like that, we just headed straight to the conference, let the games begin!

![PHPBEnelux, Welcome and enjoy the show!]({{ site.baseurl }}/images/openning.jpg)

##Friday

The checkin process was nice and easy, and we were met with a large amount of fruit and drinks (Including precious coffee that I hadn't had yet) which were openly welcomed after the amount of walking we'd done looking for breakfast. We (foolishly) thought if we looked around long enough, we'd find somewhere that did an English style breakfast, but that didn't work. McDonalds do breakfast, but we didn't realise till after we'd settled for regular food.

Anyway. The conference.

###Keynote: Talmudic Maxims to Maximize Your Growth as a Software Developer - Yitz Willroth

The opening Keynote was brilliant, and really spoke to me on a lot of levels, it was just the best start to the conference I could have asked for. I even attempted to do sketch notes (even though I can't draw) which didn't turn out *that* bad, but I suppose you can judge that for yourself.

![My attempted sketch notes]({{ site.baseurl }}/images/sketch-notes.jpg)

I took a lot of lessons from the talk, things from pair programming, [up-for-grabs](http://up-for-grabs.net), [php mentoring](http://phpmentoring.org), and many other things. At the start of the talk, Yitz tried to make us pick just one thing to take away from the talk and try and achieve. I'm Sorry, Yitz, but I took far more than one thing, I hope that's alright. It's quite clear though...

<blockquote class="twitter-tweet" lang="en"><p>It&#39;s safe to say, Yitz most definitely gets it! What a keynote <a href="https://twitter.com/hashtag/phpbnl15?src=hash">#phpbnl15</a></p>&mdash; Chris Kemper (@ChrisDKemper) <a href="https://twitter.com/ChrisDKemper/status/558619940828495873">January 23, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

###PHP Performance Tuning: Prepare for Ludicrous Speed - Davey Shafik

I got a lot of benefit out of this talk, because for some reason (I know, I know) I'd never looked at profilers before, so seeing the power that's available was very useful to me, as well as being able to see the gains it can bring. 

I was half expecting there to be more low-level optimisations given the title of the talk, but we covered a lot on XHProf, and because I'd never covered it, or any other profilers before, this was really useful to me, and I came away wanting to install all of the profilers!

![Profile, all of the things](https://i.imgflip.com/h5pim.jpg)

###Low-Level PHP: Getting started with Go - Benjamin Eberlei

This talk was brilliant for me. I got a great understanding of the basics of Go, and got reminded of a few things I'd forgotten. The overview to Go was brilliant, especially how to work with threading, and how easy it is to actually get going.

One thing in particular was, when you're coding something new, it's alright to leave everything in one file and not organise it as you would a language you're familiar with. I keep thinking I'd need to have everything looking nice, but then I remember my first HTML and PHP files were both far too many lines long, it just works for me. Also, Benji shares the same view I do on coding things for no reason, there needs to be a purpose, and with Go and it's awesome concurrency, I'm sure I'll find a use for it very soon.

###Hallway track

I took a little break after this, and decided to explore the conference a little bit. Sadly for me, I'm just not there yet when it comes to creating conversations out of nothing, so I didn't really talk too much. I did however go and see the [Continuous PHP guys](https://continuousphp.com/) and built myself an ElePHPant (although I forgot the ears), I also had a go on the [Sparkcentral](http://www.sparkcentral.com/) drone, I wasn't very good at flying that.

![My attempt at a Lego ElePHPant]({{ site.baseurl }}/images/elephpant.jpg)

###Handling Highly Connected Data with the Neo4j Graph Database - Michelle Sanver

I've been wanting to play with Neo4j for ages now, but when I couldn't get the thing installed, I'd decided to give up, so this was just what I needed. I hadn't realised how easy it was to get started and get some data in the with the WebUI, and the query language (Cypher) is nice and easy to use, which also makes things a lot easier.

Michelle mentioned [OmNomHub](https://github.com/Omnomhub/omnomhub) in the talk, which is a really cool use of Neo4j which, as the repo calls it is: "Like github! But for recipes :)" and it's worth checking out.

The biggest thing I got from the talk (Other than a much needed Neo4j intro) was the inspiration to do my own, so at PHPNE, I'll be doing a Neo4j talk some time soon!

###The infamous Friday Social

I got into the social first, so I got myself a drink and camped next to the Digital Ocean Simulator. Now, this is where I was an idiot. I saw people showing up with chips, so I was like, wtf? I looked around loads but couldn't see them. I'd messaged the guys but got no reply (we were communicating via Slack) so I just kept walking. After a while, I found the guys and they tell me the chippy van is outside. I really should have had the balls to ask someone, I need to work on that.

I grabbed a beer with the guys and we looked around. I finally had a go on the wave machine (I'd been waiting so the guys could see me fall off.) I popped a balloon when I fell off, it was awesome. I managed to grab a Digital Ocean T-shirt as well (I have a thing for [T-shirts](http://instagram.com/chrisdkemper)) so we hit the tables (Casino tables, that is) with our Benelux Bucks. We wanted to leave quite early, so I wasn't very strategic with my betting, I went big on a couple of numbers on roulette (I should have played poker) and lost pretty quick. Sterling lost his quite quick as well, and we waited for Peter by the punching machine. I was getting steady 750-790's but I never broke 800. As I always do before I quit something after I've tried a million times (figuratively, of course) I said, "One more go," or on occasion, "Uno mas." I gave it one more, and got an 811! I was happy and said something like "I quit, I'm done" holding my hands in the air. I did have a couple more go's but they were only for fun, I was just happy I'd gotten it when Id said, "One more go". We finished our drinks and left, and headed back to the hotel.

![811, I'm happy with that punching machine score!]({{ site.baseurl }}/images/punching-machine.jpg)

During the day I'd been on about making a Vagrant box with Neo4j so I could tinker with it, and Sterling said, "We'll hack on it later if you want?" I did want to, so back at the hotel, thats what we did. We managed to get the box up and running with Neo4j with a single script (Nothing wrong with doing things in one file) but we couldn't get the admin interface to show up, after trying what seemed like everything. We called it a night and headed to bed, we had an early start in the morning.

##Saturday

We got up nice and early and headed to the conference. I only had a hoody and a jumper with my, and before I actually got up, all I could hear was heavy rain. Turns out when we got outside, it was snowing. I thought being English "Ah, this'll never lie". Oh how wrong I was. We got the bus fun, the snow didn't bother the public transport at all (even though the snow was quite thick at this point) so we got to the stop for the conference without issue. The walk to the conference was lovely, I really enjoyed the snow, it was good snowball snow. I had to make one, just to be sure.

![I do love a snow covered house]({{ site.baseurl }}/images/snow-house.jpg)

We got to the conference and ended up being the first people there. We ended up playing pool until the first talk, being sure to get plenty juice and coffee beforehand.

###Migrating to DDD - Anatoly Pulyaevskiy

This talk was a good start to the 2nd day for me. I really enjoyed that it was built around an example rather than theory, and the content was brilliant. I left that talk with a much better understanding of how DDD worked, and that you can even migrate to it slowly over time.

I did have a question, but didn't have the balls to ask it, I really need to work on that.

###More hallway track

After the first talk, I wanted to get the Neo4j box working, so I took time out from the talks and went to hack on it some now. Eventually, I found the reason for the problems, more specifically, this line:

```
org.neo4j.server.webserver.address=0.0.0.0
```
By default, the webUI binds to localhost, so unless the above is commented out, it would never be available outside of the vagrant box, problem solved. After sharing my win, I then put the now working box on [GitHub](https://github.com/chrisdkemper/neo4j-vagrant), and I even tweeted about it. Since then, the box has been updated to work with Puppet, thanks to a Pull Request from [Sterling](https://twitter.com/anthonysterling).

<blockquote class="twitter-tweet" lang="en"><p>I fancy playing Neo4j, so I’ve put a very basic Vagrant on GitHub, it works, but it needs improving <a href="https://t.co/O536ULODCz">https://t.co/O536ULODCz</a> <a href="https://twitter.com/hashtag/phpbnl15?src=hash">#phpbnl15</a></p>&mdash; Chris Kemper (@ChrisDKemper) <a href="https://twitter.com/ChrisDKemper/status/558935226035220480">January 24, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

###Small Uncontrolled Experiments - Mathias Verraes

This talk was fantastic, and my other main standout talk from the conference as a whole. If you haven't seen Mathias speak before, then you really need to. No matter what the subject matter is, he always delivers a brilliant and funny talk, and this was no exception.

The idea of everything being a small experiment was brilliant, and that it's alright to fail. You never really know until you try, so why not just try it? If you realise it's not working after a week or two, scrap it. If you realise the experiment was a huge success, then make it a rule.

The main point I took away from this brilliant talk was:

> Experiments are better than opinions, always!

If you have an idea and you can try it easily, then just try it, what's the worst than can happen. Also, you don't always have to focus on what isn't working, also focus on what is working, and ask yourself:

> What's going well, what's helping be better right now?

If you realise you benefit from hot desking, or pairing, then do that more, focus on the good. 

It really was a brilliant talk. 

###Microservices: Packs small, plays BIG! - Stephan Hochdörfer

Before this talk, I had a vague understanding of Microservices, well at least the core concept, so after I feel as though I gained a lot of clarity. The talk itself was well delivered, but sadly lacking in actual examples or sadly experience when it came to questions. To be fair to Stephan, he had to field a fair few questions, and just sadly had a lack of experience. The questions mainly centred on having a shared data store, and how to keep state/speed through the different services. Clearly, Stephan knew his stuff, that was clear, just had a lack of hands-on experience with Microservices communicating together.

There was still a big case for using microservices in a legacy applications however, which was a great positive in the talk. Microservices can allow you to refactor a small piece of a legacy application, keeping the response/request the same, but isolating that services features as close as possible, keeping the size, well, micro. This allows you to do partial refactors, and the rest of the application isn't affected by the change, other than hopefully being a little faster for the optimisation. 

###Building a scalable system for tracking Shipping Packages - Premshree Pillai

Before this talk, I was more aware of Etsy for its shop rather than its tech, so when the show of hands at the start showed the majority were the opposite, I figured I better pay attention. It was really interesting to see all the usage stats for Etsy, and that it's backed by PHP. The talk was really well delivered and it made me really pay attention to the content. As we walked through the code, it seemed a lot of problems were coming from one thing, the queue.

Etsy's queue system is made with DB tables, and there were a number of tasks running to keep the numbers within these queues manageable. It seemed to me (I could be completely wrong here) but if RabbitMQ was used, then the DB tables could essentially be queues, and it would function in a similar way, but a lot of the queue logic could be removed in the app, making the core codebase cleaner. This is all theoretical of course, I have no way of knowing if it would in fact, make things better, I've just been learning a lot about RabbitMQ recently, it seems it would be ideal here.

###Say What? Ubiquitous Language and You! - Beau D. Simensen

This talk gave a brilliant overview on Ubiquitous Language and was delivered by an equally brilliant speaker. It's easy to think that Ubiquitous Language just applies to the code, but it's outside of that too, anywhere where your feature is written, coded, spoken or diagrammed, Ubiquitous Language must be used.

Luckily for me and the project I'm working on, working out what the Ubiquitous Language is, isn't really an issue. I did however get a lot of tips on how to do this if it comes up, such as just trying to get the clients to decide on a word for clarity for yourself, when in fact they're deciding on the Ubiquitous Language on their own.

When the questions came, they were all answered brilliantly, which was really good to see. My only criticism of the talk was that there no proper examples on say, what the old name was, and what it became, but other than that, a brilliant talk, by a brilliant speaker, who even thanked me for leaving feedback.

###Closing

Its safe to say the closing part of PHPBenelux was just as entertaining as the rest. The brilliant stage presence can't be ignored (Jeroen and Thijs, I'm looking at you.) and I do love a good blooper (Closing video kinda crashed, but it's on [Vimeo](http://vimeo.com/117694237) now) but all in all it was brilliant. I didn't win any prizes this time, but I didn't mind so much, although whoever won the PS4 was more excited than everyone else put together. After the sponsors had been thanked, it was time for the closing show, closing *magic* show that is. Well, before the show kicked off, there was a few times that the curtains opened and closed, much to the amusement of the crowd, and me apparently. 

I love a good magic show, so it was really cool for me, although I had no idea what the guy was saying, but I just watched everyone else turn their hands over and stuff, it looked fun!

After the magic show was over, we headed back to the main area for some <del>food</del> beer. The queues for food were rather long, so we ended up going through our drinks vouchers relatively quickly, and got thirsty for more beer. After another try on the punching machine (I nearly broke my hand again) and a brief chat, we headed to a nearby bar to grab a couple of beers.

The three of us ended up talking about ways we could use what we'd learned at the conference at home which turned out to be one of the great benefits I'd gotten out of the conference. After a lot of talking, and a few more beers, we headed back to the hotel via the very reliable (and late running, apparently) bus service.

We had an early start in the morning, so no hacking at the night time, straight to bed.

##Sunday

After we watched the closing Benelux video, we headed out for the train to head back to Brussels. It's still so weird to me that the day doesn't start till so late in Brussels, we got the train at a very empty Antwerp station, which again was very odd. The two floors of train tracks however, that was pretty cool.

If you are ever in Brussels and looking for a decent bar (with good WIFI) then check out The Big Game Brussels Sports Bar, its pretty cool.

I could fill this part with images, but I feel as though I've used enough already, but Brussels is beautiful place, and I'd love to come back. One bonus of it being so cold in Brussels, was that when I got back to Newcastle, it felt tropical, so walking round in a T-shirt was nice and refreshing, thanks, Brussels. Ok, maybe just one...

![Sterling and Wardle]({{ site.baseurl }}/images/those-two.jpg)

##All in all

For me, this conference was amazing, from start to finish. I learned so many different lessons, and because of the inspiration this conference gave me, I'm doing a PHPNE talk on Neo4j, and I may be writing another book, so it's all very exciting! It's made me realise how much you can get out of conferences when you're both inside, and outside of the tracks, or even after the conferences itself. 

I know now, I feel very inspired, and I think, that's all that really matters when it comes to it.

NOTE: I've supplied everyone I've mentioned in this post feedback on [joind.in](http://joind.in) :)