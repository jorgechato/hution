# Hution a [notion](https://www.notion.so/) like theme 
## Installation & Update
```bash
$ # install
$ git submodule add https://github.com/jorgechato/hution.git themes/hution

$ # update
$ git submodule update --remote --merge
```
If you want to know more information, see Hution doc.

## Usage

> IMPORTANT: Any post create with a date in the future will be treated as draft and filter out from the post list.
> If you want to set up the size of the images use `width`

### `config.toml` example

```toml
theme = "hution"
baseurl = "https://example.com/"
title = "Hution Themes"
paginate = 3
languageCode = "en"

enableEmoji = true
# Optional
# If you use googleAnalytics, you set top-level options in config.toml to the beginning of the config file like other top-level options.
googleAnalytics = "UA-XXXXXXXX-XX"
# and disqus too.
disqusShortName = "yourdisqusshortname"

[params]
mainSections = ["post"]
customCSS = ["/custom.css"]
favicon = "/img/favicon.png"
color = "#FFFFFF"

# Router
[permalinks]
post = "/posts/:title"

[Author]
name = "Jorge Chato"

[taxonomies]
author = "author"
tag = "tags"
category = "categories"

# copy paste this block and change for each social media to add how many ever social media
# acounts/links you want
[[params.social]]
  name="name of social media"
  url="link to social media"
  icon="A icon from https://fontawesome.com/"
```

## Posts

```md
---
title: ""
date: "2020-04-23T14:17:03Z"
author: ""
categories:
- hack 
tags:
- hack
toc: true
thumbnail: ""
summary: ""
---

# Introduction ...
```