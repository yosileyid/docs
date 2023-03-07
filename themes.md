---
layout: default
title: Jekyll Themes
---

***

I really enjoy creating jekyll themes. If you have jekyll installed already you can simply install any of my themes as a gem `gem install jekyll-newspaper` for example and use it in your existing site. For now both links in the top nav go to this page, I am splitting it up so the theme docs are more detailed. Each theme has a different type of configuration. You will see what that means eventually as the docs grow. 

{: .list-unstyled}
* `jekyll-docs-dark:`
  - This is a documentation theme for jekyll, you are seeing it live right here. 
* `jekyll-newspaper-0.2.0:` 
  - This theme resembles a Newspaper type blog.
* `jekyll-resume-0.0.1:` 
  - This is a simple bootstrap resume site for developers to use.
* `jekyll-bs5:` 
  - This is just the bootsrap v5.3 starter template, my very first theme. 

The main source of info for any jekyll theme is in the configuration file. Below you can see an example that I use as the base config file in all my themes until I decide to change the way the site works.

## Config.yml

The `_config.yml` is the most basic part of any jekyll site. It tells jekyll what information to display along with what plugins you are using and more according to what the designer has included in there.

{: .accent .rounded .text-dark}
```yaml
# Needed for gh-pages sites
#
# repository : username/repo
# github     : [metadata]

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
# ==========================================================
#
# TITLE
#
# This is the title of your "Newspaper" for example, "The Moo York Times" :)

title: Yosi's Documentation Site

description: >- # this means to ignore newlines until "baseurl:"
  This is my documentation site hosted on Github pages where you can find information about my projects.

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

baseurl       : ""

# URL
#
# This is the base hostname & protocol for your site, 
# as you see I use https://yosileyid.github.io because this
# is a template and served live on my gh-pages site.
#
# You should change this to your sitename or there will be 
# issues in links.
#
# Use localhost for local development
# http://localhost:4000


url            : "http://localhost:4000"

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
    support_server : hdg-discord
    join_server    : https://discord.gg/KpGXAEnVnv
    add_user       : https://discordapp.com/user/hasidic.dev#0613

# EXCERPT_SEPARATOR
#
# This is used in your blog posts, you can see an example in any 
# of the example blog posts included in this theme. It functions
# to trim your posts when displaying them so it doesnt show the
# entire post like on the front page. Feel free to change where
# the excerpt ends.

excerpt_separator: <!--more-->

# Build settings
#
# These are build settings needed for when you run "jekyll serve"
# commands. You can change these, but be careful because they can
# cause your site to break.

#plugins:
#  - jekyll-feed

collections:
  categories:
    output: true
    permalink: /:categories/:title/
#  authors:
#    output: true

```