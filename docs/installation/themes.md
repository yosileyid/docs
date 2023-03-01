---
layout: default
title: Installing A Theme
parent: Installation
nav_order: 2
---

# Installing a gem-based theme

{: .warning }
> This is just the tutorial from Jekyll. If you run into any issues feel free to hit me up on slack or discord and I will help you out.

The `jekyll new <PATH>` command isn’t the only way to create a new Jekyll site with a gem-based theme. You can also find gem-based themes online and incorporate them into your Jekyll project. For example, search for [jekyll theme on RubyGems](https://rubygems.org/search?utf8=%E2%9C%93&query=jekyll-theme) to find other gem-based themes. (Note that not all themes are using `jekyll-theme` as a convention in the theme name.)

## To install a gem-based theme:

### Add the theme gem to your site’s `Gemfile`[^1]:

```
# ./Gemfile

# This is an example, declare the theme gem you want to use here
gem "jekyll-theme-minimal"
```

> Or if you’ve started with the `jekyll new` command, replace `gem "minima", "~> 2.0"` with the gem you want, e.g:

```
# ./Gemfile

- gem "minima", "~> 2.5"
+ gem "jekyll-theme-minimal"
```

### Install the theme:

```
bundle install
```

### Add the following to your site’s `_config.yml` to activate the theme:

```
theme: jekyll-theme-minimal
```

### Build your site:

```
bundle exec jekyll serve
```

> You can have multiple themes listed in your site’s `Gemfile`, but only one theme can be selected in your site’s `_config.yml`.

---

#### Footnotes:

[^1]: If you’re publishing your Jekyll site on GitHub Pages, note that GitHub Pages supports only some gem-based themes. GitHub Pages also supports using any theme hosted on GitHub using the remote_theme configuration as if it were a gem-based theme.