# sunshine

A lovely theme for [Hexo].

![litten-qrcode](https://img3.doubanio.com/view/status/median/public/8d3d6d52c23065d.jpg)
![litten-qrcode](https://img3.doubanio.com/view/status/median/public/e7e76b757169686.jpg)

- [Preview](http://fiowind.top)

## Installation

### Install

``` bash
$ git clone https://github.com/fiowind/hexo-theme-sunshine.git
```

**sunshine requires Hexo 2.4 and above.**

### Enable

Modify `theme` setting in `_config.yml` to `hexo-theme-sunshine`.

### Update

``` bash
cd themes/hexo-theme-sunshine
git pull
```

## Configuration

``` yml
# Header
menu:
  Home: /
  Archives: /archives
rss: /atom.xml

# Content
excerpt_link: Read More
fancybox: true

# Sidebar
sidebar: right
widgets:
- tag
- about
- archives
- recent_posts

# Miscellaneous
google_analytics:
favicon: /favicon.png
mywords: 
weibourl: 
githuburl:
facebookurl: 
zhihuurl: 
```

- **menu** - Navigation menu
- **rss** - RSS link
- **excerpt_link** - "Read More" link at the bottom of excerpted articles. `false` to hide the link.
- **fancybox** - Enable [Fancybox]
- **sidebar** - Sidebar style. You can choose `left`, `right`, `bottom` or `false`.
- **widgets** - Widgets displaying in sidebar
- **google_analytics** - Google Analytics ID
- **favicon** - Favicon path
- **twitter** - Twiiter ID
- **google_plus** - Google+ ID

## Features

### Fancybox

sunshine uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### Sidebar

You can put your sidebar in left side, right side or bottom of your site by editing `sidebar` setting.

sunshine provides 5 built-in widgets:

- category
- tag
- tagcloud
- archives
- recent_posts

All of them are enabled by default. You can edit them in `widget` setting.

## Development

### Requirements

- [Grunt] 0.4+
- Hexo 2.4+

### Grunt tasks

- **default** - Download [Fancybox] and [Font Awesome].
- **fontawesome** - Only download [Font Awesome].
- **fancybox** - Only download [Fancybox].
- **clean** - Clean temporarily files and downloaded files.

[Hexo]: http://zespia.tw/hexo/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
[Grunt]: http://gruntjs.com/

