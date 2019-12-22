---
title: "Hugo & Firebase work well together"
date: 2019-01-10T00:21:58Z
draft: true
---

So I've been playing around a little bit with [Hugo](https://gohugo.io) and [Firebase](https://firebase.google.com) - that's what this new site is built with. It is also the first time I've played around with [text/markdown](https://en.wikipedia.org/wiki/Markdown) to build a website.  Not a bad combination to build a static page based structure and you can see that I have gone to town on with a [simple hugo theme](https://github.com/Xzya/simple-hugo-theme) inspired by the geniuses behind [bettermotherfuckingwebsite.com](http://bettermotherfuckingwebsite.com).

It wasn't super hard to get it all together.  Here are the steps I took...

**1.** Download and configure [Hugo](https://gohugo.io) with the [simple hugo theme](https://github.com/Xzya/simple-hugo-theme) - here's a trick... create your Hugo directories FIRST!

```bash
hugo new site krandor
cd krandor/themes
git clone https://github.com/Xzya/simple-hugo-theme.git simple
cd ..
vi config.toml
hugo new about.md
hugo -t simple -D
```

**2.** Create a Firebase Hosting site - see [Get started with Firebase Hosting](https://firebase.google.com/docs/hosting/quickstart) - initialise your Firebase project in your 

```bash
firebase login
firebase init
firebase deploy
```

**3.** Check out the site and browse to the `/about` path
