# Ink

Minimal website and blog theme Hugo. Forked from [ink](https://github.com/knadh/hugo-ink).

## Demo

![Screenshot](https://www.dropbox.com/s/izst24s2v01dtpy/Screen%20Shot%20Github%20HugoLog.png?raw=1)

## Features

- Google & Plausible Analytics integration
- SEO optimization
- Syntax highlighting
- Twitter cards and opengraph tags support
- Disqus comments
- RSS feeds
- Custom CSS/JS
- Multilingual months support

## Installation

cd into your hugo site's root directory and:

```sh
cd themes
git clone https://github.com/angezanetti/hugo-dot.git
```

For more information read the [official setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Content type

You can specify content type with field `type` in your content. For example static pages can be set as type `page` which are excluded from recent posts and all posts page. You can use site params `mainSections` and `disableDisqusTypes` to control which page types are excluded from recent posts and Disqus comments respectively.

```md
---
title: My Title
date: 2020-11-13T09:40:23-04:00
description: My description
draft: false
tags:
  - tag1
  - tag2
---

This is some static page where you can write about yourself.
```

## Language Settings for the month

Due to the currently unavailable feature for multilingual dates in `.Date` from
Go. It is possible to create a `month.yaml` in the data folder of your
Hugo site root directory. There is also an example file in
`exampleSite/data/`.

```sh
cat > month.yaml << EOF
1: "Jan"
2: "Feb"
3: "Mar"
4: "Apr"
5: "May"
6: "Jun"
7: "Jul"
8: "Aug"
9: "Sep"
10: "Oct"
11: "Nov"
12: "Dec"
EOF
```

## Credits

- [ink](https://github.com/knadh/hugo-ink).

Licensed under the MIT license.
