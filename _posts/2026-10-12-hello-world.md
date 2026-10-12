---
layout: post
title: Hello, world
date: 2026-10-12 09:00:00+0900
description: The first note, and how new notes get added here
tags: meta
categories: notes
---

This is where I write down what I learn. Short, informal, and mostly for my future self.

## How a new note is added

1. Create a file in `_posts/` named `YYYY-MM-DD-title.md`.
2. Start it with front matter like this:

   ```yaml
   ---
   layout: post
   title: Note title
   date: 2026-10-12 12:00:00+0900
   description: One-line summary
   tags: tag1 tag2
   categories: notes
   ---
   ```

3. Write the body in Markdown and push to `master`. The site rebuilds and deploys automatically within a few minutes.

Math works too:

$$
E = mc^2
$$
