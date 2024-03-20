---
title: "Create your own Hugo site and deploy it with Cloudflare Pages with ease!"
summary: "Create your own Hugo site and deploy it with Cloudflare Pages with ease!"
date: 2024-01-31
aliases: ["create-hugo-cloudflare-pages"]
tags: ["hugo", "cloudflare", "pages", "cloudflare pages", "tutorial", "draft"]
author: "Hanif Al Fathoni"
draft: true
hidemeta: false
comments: false
searchHidden: true
showToc: true
cover:
    image: /hugo-cloudflare.png
    alt: "Hugo + Cloudflare Pages"
    relative: false
    hidden: false
---

## Introduction

In this tutorial, we will learn how to create a Hugo site and deploy it with Cloudflare Pages with ease!

## Introduction to Hugo

<!-- Hugo logo -->
![Hugo logo](https://gohugo.io/images/hugo-logo-wide.svg)

Hugo as they called it as "The world’s fastest framework for building websites". Hugo is a static site generator written in Go. It is optimized for speed, easy use, and configurability. Hugo takes a directory with content and templates and renders them into a full HTML website.

To install Hugo, you can follow the official documentation [here](https://gohugo.io/getting-started/installing/).

## Create a new Hugo site

First, go to the directory where you want to create a new Hugo site.

Then, to create a new Hugo site, you can use the following command:
You can replace `my-site` with your own site name.

**Note:** We will use `yaml` for the format. You can also use `toml` or `json` as the format. Default is `toml`.

```bash
hugo new site my-site --format yaml
```

## Add a theme

To add a theme, you can use the following command:
For example we will use [PaperMod Theme](https://github.com/adityatelange/hugo-PaperMod).

```bash
cd my-site
git init
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive
```

**Command Explanation:**
`git init` - Initialize a git repository in the current directory.
`git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod` - Add the PaperMod theme as a git submodule.
`git submodule update --init --recursive` - Update the theme's git submodule.

## Configure the theme

The, open the directory `my-site` in your favorite code editor.

In the hugo.yaml file, add the following line:

```yaml
theme: PaperMod
```

## Add content

To add content, you can use the following command:
You can replace `my-first-post` with your own post name.

The content will be created in `content/posts/my-first-post.md`.

```bash
hugo new content posts/my-first-post.md
```

## Run Hugo server

After we add content, let's run the Hugo server to see the result.

```bash
hugo server
```

Hugo will run the server on `http://localhost:1313/` or another port if 1313 is already used (Check the terminal output).

Then, open `http://localhost:1313/` in your browser and you will see the result.

![Hugo result](/result.png)