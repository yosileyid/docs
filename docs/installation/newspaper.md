---
layout: default
title: Installing Newspaper
parent: Installation
nav_order: 3
---

# {{page.title}}

![Screenshot 2023-02-27 2 25 57 PM](https://user-images.githubusercontent.com/14003326/221665661-bea2e406-aac4-480c-9b6c-c4cb68a125fb.png)

## Download the ZIP file:

You can download the full theme as a zip file [here]() then simply extract it locally and in your terminal CD into that directory. You will need to run `bundle install` first to ensure everything is installed and then you can run `bundle exec jekyll serve` and you should be able to go to http://localhost:4000 and view your site.

## Installing as a Gem:

Once you have Jekyll and some theme set up and your site is running it is a simple process to install the `jekyll-newspaper` theme. All you need to do is edit your `Gemfile` and where it says `gem "minima"`, change that to `gem "jekyll-newspaper", "~> 0.0.1"`. Then in your `_config.yml` add a line like so:

```yaml
theme: jekyll-newspaper
```

After you have that saved, you do `bundle install` and then `bundle exec jekyll serve`, you should see something similar to the image below:

![Screenshot 2023-02-26 6 59 54 PM](https://user-images.githubusercontent.com/14003326/221446384-5cca3f1d-4343-4931-bee2-d7b2537d18d4.png)

If there is an issue send me an email or join me on discord or slack and I will help out if I am able.