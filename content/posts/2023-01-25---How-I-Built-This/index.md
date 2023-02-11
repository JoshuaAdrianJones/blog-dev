---
title: How I built this blog
date: "2023-01-25"
template: "post"
draft: false
slug: "/posts/How-I-Built-This"
category: "Software"
tags:
  - "Software"
  - "Blog"
  - "GatsbyJS"
description: "A Super simple guide to building a blog with gatsby and using github-pages to host."
socialImage: "./media/gatsby.png"
---

## A Super simple guide to building a blog with gatsby and using github-pages to host:

This article is mainly my personal notes for GatsbyJS and the lumen starter.

### What is GatsbyJS?

[A static site generator for ReactJS](https://www.gatsbyjs.org/)

### What is Lumen?

A minimal, lightweight and mobile-first starter for creating blogs using Gatsby.

### Getting set up

- Install node [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
- Install gatsby

  ```sh
   npm install -g gatsby-cli
  ```

### Create a Gatsby site

Use the Gatsby CLI to create a new site, specifying the Lumen starter.

```sh
gatsby new blog https://github.com/alxshelepenok/gatsby-starter-lumen
```

### Start Developing

Navigate into your new site’s directory and start it up.

```sh
cd blog
npm install
npm run start
```

## Open the source code and start editing!

Your site is now running at `http://localhost:8000`!

## How to actually edit stuff the simple way

There are a bunch of files and folders in the /blog/ folder that are needed to build the site, to actually edit the blog to your own content there are a small number of folders and files you actually have to edit.

### Important files and folders

- /content/pages holds the about and contact pages, and any other pages you might want to add.

- /Content/posts holds the blog posts

- /config.json holds the meta data for the site and social media accounts

### Developing

- You can make edits to blog posts `(.md)` files and save and the localhost:8000 page in your browser will auto-load your changes.
- To see edits to config.js you need to stop the `npm run start` command (usually ctrl+c in your terminal) and run it again.

### Publishing to github pages

- npm run deploy < - this builds the site to the `/public ` folder this is the folder to upload to github pages.
- move the contents of public to your gh-pages repository and the site will build from there in a few minutes.
