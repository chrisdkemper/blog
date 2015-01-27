---
layout: post
title:  "Load the 'Main menu' for Drupal 7 in code"
date:   2015-01-28 12:25:09
comments: true
categories: drupal7 drupal
summary: A code snippet to load Drupal 7's default Main Menu in code
---

There comes a time when you need to load a menu directly into the code on a Drupal project, and there's a lot of guides to do this.

When I was looking around though, I couldn't find a single one on loading the actual 'Main menu' that Drupal creates, so after working out how to do it, I figured I'd share.

The main issue with it being created by the `system` module rather than the `menu` module, but either way, here's a Gist

{% gist chrisdkemper/4746c2d36ffa42f18f47 %}

