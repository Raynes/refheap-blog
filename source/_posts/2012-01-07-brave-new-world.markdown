---
layout: post
title: "Brave New World"
date: 2012-01-06 19:45
comments: true
categories:
---

[RefHeap](http://refheap.com) (short for Reference Heap) is a pasting website. It is being built by myself ([Anthony Grimes](http://github.com/Raynes)) and [Alex McNamara](http://github.com/amcnamara). You may know us (him in particular) as contributors to the popular Clojure learning website [4Clojure](http://4clojure.com).

RefHeap is built with [Clojure](http://clojure.org) and uses a lot of fantastic tools. We are taking advantage of awesome technologies such as [MongoDB](http://www.mongodb.org/), the [Noir](http://webnoir.org/) web framework, and the excellent [Pygments](http://pygments.org/) syntax highlighting tool.

Development on this service began right around two weeks ago. Today, Alex and I are excited to launch this website. It has been running at <http://refheap.com> for the majority of those two weeks and we have been using it ourselves. We feel that it is currently stable and useful enough to make available to the public.

## Why?

Ruby has [Pastie](http://pastie.org), Haskell has [HPaste](http://hpaste.org); even Factor has its own [pastebin](http://paste.factorcode.org/). Clojure has nothing. That was my original motivation — to develop a pastebin that the Clojure community can call its own. That is still a goal, but we want to do more than that.

RefHeap is meant to be a language-agnostic pastebin. Backed by Pygments, RefHeap supports over 120 languages/formats right now. As Pygments grows, so will RefHeap's language support.

There are certainly a lot of tools out there for pasting. We think that a lot of them leave something to be desired, and we want RefHeap to fill those holes.

## What We Have

We currently have what we feel to be an excellent pastebin as it stands.

* With support for over 120 languages, we already support more than [Pastie](http://pastie.org).
* A UI that doesn't slap you in the face.
* A full featured and documented [API](http://refheap.com/api).
* A [Clojure library](https://github.com/Raynes/innuendo) for that API.
* Private pastes.
* User accounts that give you your own user pages with a list of your public pastes (and your private pastes when you alone are looking).
* The easiest login/register flow ever thanks to our support of the excellent and new [BroswerID](http://browserid.org).
* Syntax highlighting that is easy to look at.
* Editing and deletion of pastes that you own.
* Ability to embed pastes in your own websites/html (similar to what gist does).
* A full-screen view of a paste. Have you ever used htmlfontify in Emacs to dump a buffer (syntax highlighting/background and all) to an HTML file? Picture that.
* A raw view of a paste.
* Forking. Similar to gists, we want users to be able to hit a single button and get a copy of a paste on their own account.
* SSL. The site automatically redirects non-https traffic to https, just like gist. We care about your privacy too.

## What We Want

We have a ton of [issues](http://github.com/Raynes/refheap/issues) on Github and  almost all of them are planned features. In particular, these things are coming soon:

* Even prettier syntax highlighting.
* All kinds of statistics and information about pastes. Number of them, number of them by language, etc.
* Revisions. Also similar to gists, we want to keep revisions of all edits you've made on a paste. When you fork a paste, these will come with it.
* Diffs on revisions and perhaps the ability to roll back changes.
* Searching/filtering pastes.

A lot of these things are mostly trivial and will be appearing very quickly now that we've got the really important and hard stuff done. Want more? Tell us!

## Conclusion

RefHeap is already pretty cool, but we're working hard to make it *awesome*. We want you to be a part of it. Here are some things you can do to help:

* If you find any bugs or feature requests, please file issues for them on [Github](https://github.com/Raynes/refheap/issues) if they don't already exist. 
* Contribute. If you're a Clojurian or have experience with web design and want to help out, please do! This site is completely open source.
* Tell your friends about us. Simply *use* the site! Just spreading links is a great way to spread the word. You can also tweet about us.
* Come join in the fun on IRC in the #refheap channel on the Freenode IRC network. This is where all the developer chat goes on and Alex and I are almost always around. We don't mind some casual conversation as well. This is a great place to touch base and talk with the developers if you plan to contribute.
* Write libraries/tools with our API. We have a full [API](http://refheap.com/api). The lazybot IRC bot that you can find in the #clojure IRC channel already uses refheap for pasting. [4Clojure](http://4clojure.com) will be using it soon. You should too! We have our API library in Clojure, but we want to see libraries for all sorts of languages! Stake your claim and write one. Seriously, go do it now.
* Follow us on Twitter [@RefHeap](http://twitter.com/RefHeap).

This is it. Enough talking. We're launching this sucker. We really like how RefHeap is turning out, and we hope you do too. Now go forth and paste!

Sincerely,

Anthony Grimes and Alex McNamara.

**update**

I updated a sentence near the top where I originally said the site was built from the ground up in Clojure. Some people felt that I was being insincere because we actually use Pygments on the backend for syntax highlighting. We use a *lot* of great tools on the backend. I don't want to imply in any way that Clojure is our sole tool.
