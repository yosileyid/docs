---
layout: default
title: Installing Jekyll
parent: Installation
nav_order: 1
---

## Installing Jekyll

#### Ubuntu Linux:

I use and develop on Linux systems so I can help you in chat if there are any issues installing. 

Install Ruby and other prerequisites:

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your ~/.bashrc file to configure the gem installation path:

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Finally, install Jekyll and Bundler:

```
gem install jekyll bundler
```

That’s it! You’re ready to start using Jekyll. Now read the link titled "Installing A Theme" to install a basic default theme. Minima is the theme jekyll ships with. It has only a couple pages and needs customizing to work, so next I will walk you through the process of editing that theme when you run `jekyll new {sitename}` to use one of the themes I have made.