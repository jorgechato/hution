# Hution a [notion](https://www.notion.so/) like theme 
## Installation & Update
```bash
$ # install
$ cd themes
$ git submodule add https://github.com/jorgechato/hution.git hution

$ # update
$ git submodule update --remote --merge
```
If you want to know more information, see Hution doc.

## Usage
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

[Author]
name = "Jorge Chato"
# copy paste this block and change for each social media to add how many ever social media
# acounts/links you want
[[params.social]]
  name="name of social media"
  url="link to social media"
  icon="A icon from https://fontawesome.com/"
```
