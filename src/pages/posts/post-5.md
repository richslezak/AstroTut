---
layout: ../../layouts/MarkdownPostLayout.astro
title: My Fifth Blog Post
description: "Order of imports Issues I discovered while learning some Astro."
author: Astro Learner
pubDate: 2023-01-08
image:
  url: "https://astro.build/assets/blog/astro-showcase/astro-showcase-screenshot.jpg"
  alt: "Thumbnails of websites from the Astro Showcase site."
tags: ["astro", "blogging", "learning in public", "successes", "issues"]
---

I was seeing that in the social component the inline styles were being overwritten by global css. Thought it was something do to with nested components however after some debuging I relaized that I was inporting the global styles after the compnonents. I put the global css as the first import in the base layout and the issue was resolved. The take away I have learend from this is to always import globals first.
