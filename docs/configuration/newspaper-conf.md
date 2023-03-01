---
layout: default
title: Newspaper Configurations
parent: Configuration
nav_order: 1
---

# Newspaper Configurations

I tried to be wordy enough in the `_config.yml` that it would help you find the information you need, this is just a backup of those comments presented in html for viewing.

### TITLE:

This will be the `title` of your site. Change it to whatever you want to display on the title line above the hero image and across the site. 

```yaml
# This is a "Newspaper" blog theme written for Jekyll users in Bootstrap v5.03
# we create themes and plugins professionally, but we also have free themes we
# offer to the community. Feel free to edit any of the links and usernames below
# and add your own. This will be expanding to include more features as I have
# time. Feel free to contribute by joining my server and discussing how to get
# involved.
#
# If you need any help feel free to reach out on discord or email me and I will
# help in any way you need. If you want a custom theme or plugin built you can 
# hop on discord and we can discuss it.
#
# Discord: https://discord.gg/KpGXAEnVnv

# TITLE
#
# This is the title of your "Newspaper" for example, "The Moo York Times" :)

title: Bootstrap v5.3 Blog
```

### DESCRIPTION:

This is what will display across your site in every page head there is a meta tag that will display this. It is common to have something short and effective that describes what your site does. 

```yaml
description: >- # this means to ignore newlines until "baseurl:"
  This is a Bootstrap "Newspaper" blog theme written for Jekyll users. It is a work in progress and I am adding more features to it. Feel free to download it and use it as a theme for your site. Any questions you have can be answered on the Discord server linked in the "Social Links" below. 
```

### BASE URL: 

Since this is a theme on my github user page live, I have it set to `/jekyll-newspaper` since it is served up at https://yosileyid.github.com/jekyll-newspaper change the base URL to whatever directory you want it to be hosted on your site `/blog` is common. If you want this to be the home page of your site the base URL will be "/"

```yaml
# BASEURL
#
# This is the subpath of your site, e.g. /blog
# if you want users to access your site at https://example.com/blog
# if you are using a gh-pages site this will be 
# empty if your site is on https://username.github.io
# if your repo using this theme is named "foobar"
# then change this to /foobar and when you serve
# it using the pages setting it will be live at
# https://username.github.io/foobar 
# 
# I have blog posts on my site explaining these
# processes in more detail to help you. If you
# get stuck feel free to reach out.
#
# "/jekyll-newspaper/"


baseurl        : "/jekyll-newspaper/"
```

### URL:

This will be the `URL` people will use to visit your "/blog" https://example.com is the format. When developing on local machines change this to `"/"` or `http://localhost:4000` and leave baseurl empty.

```yaml
# URL
#
# This is the base hostname & protocol for your site, 
# as you see I use https://yosileyid.github.io because this
# is a template and served live on my gh-pages site.
#
# You should change this to your sitename or there will be 
# issues in links.

url            : "" # "https://yosileyid.github.io"
```

### SOCIAL:

These are social links I am using across the site in various places. Feel free to change them to your own username. 

```yaml
# SOCIAL 
#
# This section handles your social network links displayed for now
# in the Social Links section on the front page. I will add more
# as I recieve user feedback on the theme.

social:
  twitter          : hasidicdevs
  github           : yosileyid
  email            : yosi@hasidic.dev
  discord: 
    username       : hasidic.dev#0613
    support_server : "[hdg-discord]"
    join_server    : https://discord.gg/KpGXAEnVnv
    add_user       : https://discordapp.com/user/hasidic.dev#0613
```

### EXCERPTS

This is needed to trim your posts display on pages. You need to include this tag in any page or post you want to display somewhere else and have the content trimmed down.

```yaml
# EXCERPT_SEPARATOR
#
# This is used in your blog posts, you can see an example in any 
# of the example blog posts included in this theme. It functions
# to trim your posts when displaying them so it doesnt show the
# entire post like on the front page. Feel free to change where
# the excerpt ends.

excerpt_separator: <!--more-->
```

### BUILD SETTINGS:

I wouldn't change these unless you know what they do.

```yaml
# Build settings
#
# These are build settings needed for when you run "jekyll serve"
# commands. You can change these, but be careful because they can
# cause your site to break.

plugins:
  - jekyll-feed

collections:
  categories:
    output: true
    permalink: /:categories/:title/
  authors:
    output: true
```