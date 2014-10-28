---
layout: post
title:  "A new site, eventually "
date:   2012-06-10 11:39:09
comments: true
categories: frontend
---

Since my previous site, a placeholder page I built on the Megabus home from the .net awards in 2010 I've been saying I'll build a new one, and now, I finally have! Due to this being nearly 2 years coming, I've decided to just finally get something out there actually allows me to blog, and show any potential side projects I have going on (wait and see for that one). I was initially going to build the site in Drupal, then in Wordpress, then in PyroCMS. Although all of these systems would have been perfectly adiquete, I then suddenly realised, I know how to code, I don't need a CMS.

With that in mind, I then decided to go down the framework route, in the form of Silex. If you're looking to whack a quick prototype together, or a nice little site like this one, I'd definently give it a try. To go with this, I also made use of the TWIG capabilities of Silex, and decided to serve my content in the form TWIG templates for the main layout, and Markdown files for the actual content. Although this seems like a backwards way to work, the lack of a database means the site is shockinly fast, which is always a good thing. The disadvantage of this however, is when it comes to routing, as it all has to be done manually, but that comes down to an array with a filename and a slug, so once you have a couple in there it's easy enough to work with.

On the design side of things, you may have already worked out I've went with the Twitter bootstrap as a base. This allowed me to get the site up and running really quickly, and just skin it for my needs. I decided to get it from Github, so I could have access to the LESS files, allowing me to compress all the styles into one file, which helps with the super speedyness.

To cover the comments, I've decided to go with Disqus. I've always liked using this, mainly because of the ease, and that it takes care of the moderation and annoying aspects of dealing with comments, ala spam. That pretty much sums up the site, the rest of the aspects I just added in little bits at a time, and I'll no doubt change the design when I kick off a side project or two, but theres time for that yet.

If you have any thoughts on the setup or would like to offer some suggestions, I'd love to read about them in the comments.