<p align="center"><a href="https://shen-yu.gitee.io" target="_blank" rel="noopener noreferrer"><img width="100" src="logo.png" alt="ayer logo"></a></p>

<h3 align="center">一个安静且优雅的 Hexo 主题</h3>

<p align="center">
  <a href="https://travis-ci.org/Shen-Yu/hexo-theme-ayer?branch=master" target="_blank" rel="noopener noreferrer">
    <img alt="travis-ci" src="https://travis-ci.org/Shen-Yu/hexo-theme-ayer.svg?branch=master">
  </a>
  <a href="http://standardjs.com" target="_blank" rel="noopener noreferrer">
    <img alt="js-standard-style" src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg">
  </a>
  <br>  
  <a href="https://www.npmjs.com/package/hexo-theme-ayer" target="_blank" rel="noopener noreferrer">
  <img alt="npm" src="https://img.shields.io/npm/dt/hexo-theme-ayer">
  </a>
  <a href="https://shen-yu.gitee.io" target="_blank" rel="noopener noreferrer">
   <img alt="platform" src="https://img.shields.io/badge/platform-PC--ios--android-ff69b4.svg">
   </a>
  <a href="https://gitter.im/hexo-theme-ayer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge" target="_blank" rel="noopener noreferrer">
    <img alt="Gitter" src="https://badges.gitter.im/Join%20Chat.svg">
  </a>
  <br>
  <a href="https://www.npmjs.com/package/hexo-theme-ayer" target="_blank" rel="noopener noreferrer">
    <img alt="npm version" src="https://img.shields.io/npm/v/hexo-theme-ayer">
  </a> 
 <img alt="language" src="https://img.shields.io/badge/language-ejs--stylus-green.svg">
 <a href="https://github.com/Shen-Yu/hexo-theme-ayer/releases" target="_blank" rel="noopener noreferrer">
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Shen-Yu/hexo-theme-ayer?color=b37feb">
  </a>
  <a href="https://github.com/Shen-Yu/hexo-theme-ayer/blob/master/LICENSE" target="_blank" rel="noopener noreferrer"><img alt="LICENSE" src="https://img.shields.io/badge/LICENSE-SATA-yellow">
  </a>
</p>

---

:rocket: Ayer_space is a Hexo theme adpated from [Ayer](https://github.com/Shen-Yu/hexo-theme-ayer) by shinyu. It contains a lot of nice features and several nice improvements.

<b>注：收藏本主题请点右上角Star，谢谢~~ </b>
<b>如果你想给主题添砖加瓦，可以点右上角Fork，然后给此仓库提交PR</b>

### [Preview 预览](https://foxhuntervis.com/)

![Screenshot](screenshots/hexo_theme_space.png)

### [原版预览](https://shen-yu.gitee.io/2019/ayer/)



![Screenshot](screenshots/hexo-theme-ayer.png)

## Install Original Version

Adpated version will be open soon!

### For hexo < 5.0

``` shell
git clone https://github.com/Shen-Yu/hexo-theme-ayer.git themes/ayer
```

### For hexo >= 5.0

``` shell
npm i hexo-theme-ayer -S
```

- If this theme is newly installed, a `_config.ayer.yml` file will be generated in the root directory after the installation is complete, and you can directly edit the `_config.ayer.yml` file for configuration.
- If it is a theme upgrade, you can use the configuration method of hexo < 5.0, or you can move the original configuration file to the root directory and rename it to `_config.ayer.yml`.

## Enable

Modify `theme` setting in `_config.yml` to `ayer`

``` yml
theme: ayer
```

## Update

``` bash
cd themes/ayer
git pull
```

## Multi Language Support
zh-CN（中文简体） en（English） zh-TW（中文繁体） ja（Japanese） es（Spanish） de（German） fr（French） ru（Russian） ko（Korean） vi（Vietnamese） nl（Dutch） no（Norwegian） pt（Portuguese）

English is default languge, if you want to change, modify `language` option in `_config.yml` file in your blog's root folder.

## Configuration

let me know if you have any questions.

``` yml
# Menu-Sidebar
menu:
  switch_lang: https://foxhuntervis.com/zh-CN
  home: /
  categories: /categories
  research: /categories/research
  leisure: /categories/leisure
  codes: /categories/codes
  aboutme: /about/aboutme.html

# Subtitle and Typing animation
# https://github.com/mattboldt/typed.js
subtitle:
  enable: true
  text: The Game is On!
  text2: Eadem mutata resurgo!
  text3:   #Supports up to three lines of text
  startDelay: 0
  typeSpeed: 200
  loop: true
  backSpeed: 100
  showCursor: true

# Favicon and sidebar logo
favicon: /pikachu.png
logo: /images/pokeball-side.png

# Cover Setting 
# enable: [true|false]；path: [background-image]；logo: [cover-logo-image]
cover:
  enable: true
  path: /images/spacestation.jpg # there are some beautiful cover images in Ayer's directory: /source/images, choose your favorite image to replace it.
  logo: /images/pokeball-side.png

# ProgressBar  
progressBar: true

# Boardcast
broadcast:
  enable: true
  type: 1 # 1：custom，2：hitokoto api(https://hitokoto.cn/)
  text: Happy Chinese New Year! # only work in custom mode

# Article Setting
# (Use this to excerpt if article is too long：<!--more-->)
excerpt_link: Read More...
excerpt_all: false

# Copy code button
copy_btn: true
# Share
share_enable: true
# If you are not in China, maybe you prefer to set:false
share_china: true
# share text
share_text: Share
# search text
search_text: Search
# nav text
nav_text:
  page_prev: Prev page
  page_next: Next page
  post_prev: Newer posts
  post_next: Older posts

# Catalog in article
toc: true

# images in the article support click to fullscreen
image_viewer: true

# https://github.com/willin/hexo-wordcount
word_count:
  enable: true
  # only display in article page(not in index page)
  only_article_visit: true

# Reward Setting
# type：0-close reward； 1-only open in article which you have configured reward:true； 2-open in all articles
reward_type: 2
# reward word
reward_wording: 'Buy me a cup of coffee~'
# qrcode image path
alipay: /images/alipay.jpg
# qrcode image path
weixin: /images/wechat.jpg

# Copyright
# type：0-close all； 1-only display in article which you have configured copyright: true； 2-all articles
copyright_type: 2

# Search
# https://github.com/theme-next/hexo-generator-searchdb
search: true

# RSS
# leave it empty if you dont' need
rss: /atom.xml

# DarkMode
darkmode: true

# Canvas background style: 0-close，1-moveline
canvas_bg: 0

# Custom mouse pointer，replace /images/mouse.cur
mouse:
  enable: false
  path: /images/mouse.cur

# Click effect: 0-close，1-love，2-boom，3-particles
click_effect: 0

# articleWidth and sidebarWidth
layout:
  article_width: 80rem
  sidebar_width: 8rem

# GitHub Ribbons(https://github.blog/2008-12-19-github-ribbons/)
github: 
  # (Set false if you don't need)
  enable: false
  url: https://github.com/Shen-Yu/hexo-theme-ayer

# pv&uv statistics
busuanzi:
  enable: true

# cnzz statistics
cnzz:
  enable: true
  url: #

# Google Analytics
google_analytics: ''
# Baidu Analytics
baidu_analytics: ''

# Mathjax Support
mathjax: true

# Katex Support
# note: need change the hexo-renderer，npm un hexo-renderer-marked -S && npm i hexo-renderer-markdown-it-katex -S
katex:
  enable: false # true
  allpost: true
  copy_tex: false

# since year
since: 2019

# pageFooter (Set true can let more people know this theme, Thanks!)
pageFooter: true

# only for chinese website
# ICP
icp:
  enable: false
  url: "http://www.beian.miit.gov.cn/"
  text: "浙ICP备88888888"
# gongan
gongan:
  enable: false
  img: /images/beian.png
  url: "http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=01234567890123" #link
  text: "浙公网安备01234567890123号"

# friends link
friends_link:
  Ayer: #site name
    # site url
    url: https://github.com/Shen-Yu/hexo-theme-ayer
    # site icon(optional)
    img: /images/ayer.png
  GitHub:
    url: https://github.com/Shen-Yu
    img: https://i.loli.net/2020/09/07/indb4PRYDA98EkN.png
  gitee:
    url: https://gitee.com/shen-yu
    img: https://i.loli.net/2020/09/07/K3AqO7h6krQFlRX.png
  Hexo:
    url: https://hexo.io
    img: https://i.loli.net/2020/09/07/UYGzjo7h68CRWny.png
  hexo-tag-chart:
    url: https://github.com/Shen-Yu/hexo-tag-chart
    img: https://i.loli.net/2020/09/07/GIXBYE5SoylhR1r.png

# Comment：1、Valine (recommended)；2、Gitalk；3、Twikoo；4、MiniValine
# You can close the comment section on one of your posts by marking `comments: false` in front-matter.

# 1、Valine [A fast, simple & powerful comment system](https://github.com/xCss/Valine)
# You need create leancloud account first (https://console.leancloud.app), then put the id|key in below.
leancloud:  
  enable: true
  app_id: #
  app_key: #
# Valine Setting
valine:
  enable: true 
  avatar: mp # (https://valine.js.org/avatar.html)
  placeholder: Add some comments to my article~ # placeholder

# 2、Gitalk(https://github.com/gitalk/gitalk)
gitalk:
  enable: false # true
  clientID: # GitHub Application Client ID
  clientSecret: # Client Secret
  repo: # Repository name
  owner: # GitHub ID
  admin: # GitHub ID

# 3、Twikoo(https://github.com/imaegoo/twikoo)
twikoo:
  enable: false
  envId: #

# 4、MiniValine
# See: https://github.com/MiniValine/MiniValine
minivaline:
  enable: false
  md: true
  # more options https://minivaline.js.org/docs/cn/#/Options 
  backend: waline
  serverURL: https://waline.vercel.app
```

## Plugins

+ [hexo-generator-search](https://github.com/wzpan/hexo-generator-search) (for Local Search)
	
  ```yml
  $ npm install hexo-generator-searchdb --save
  ```
  Then add the plugin configuration in hexo's configuration file `_config.yml` (note: not the theme's configuration file):
  
  ```yml
  # Hexo-generator-search
  search:
    path: search.xml
    field: post
    format: html
  ```

+ [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed) (for RSS)

  ```yml
  $ npm install hexo-generator-feed --save
  ```
  
  Then add the plugin configuration in hexo's configuration file `_config.yml` (note: not the theme's configuration file):
  
  ```yml
  feed:m 
      type: atom
      path: atom.xml
      limit: 20
      hub:
      content:
      content_limit: 140
      content_limit_delim: ' '
      order_by: -date	
  ```
  
+ [hexo-generator-index-pin-top](https://github.com/netcan/hexo-generator-index-pin-top) (for Sticky Post)
	
	``` bash
  $ npm uninstall hexo-generator-index --save
  $ npm install hexo-generator-index-pin-top --save
  ```
## Categories
``` bash
  hexo new page categories
```
Then paste following codes to file: /source/categories/index.md
``` md
---
title: categories
type: categories
layout: "categories"
---
```

## Tags
Same as categories.

## Friend Links
``` bash
hexo new page friends
```
Then paste following codes to file: /source/friends/index.md
``` md
---
title: friends
type: friends
layout: "friends"
---
```
Then edit `friends_link` in `_config.yml` 

## Gallery
Need to write in the head of the markdown, this is not a good way to write, I hope to get a better way to write on github.

``` md
---
title: Gallery

albums: [
        ["img_url","img_caption"],
        ["img_url","img_caption"]
        ]
---
```

## Toc

Use Tocbot to parse the title tags (h1~h6) in the content and insert the directory. 

+ ayer/_config.yml

	``` bash
	# Toc
  toc: true
	```
+ If Toc is turned on in ayer/_config.yml, then Tocbot will generate a Toc article directory in the title tag of each blog parsing content, but not all blogs require Toc, so in the Front-matter section of markdown Can be closed:

	``` md
	---
  no_toc: true
  ---
	```

---

<br/>

## License



#### Original Licence

```text
The Star And Thank Author License (SATA)

Copyright © 2019 Shen-Yu(shenyu@hotmail.com)

Project Url: https://github.com/Shen-Yu/hexo-theme-ayer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software. 
```

