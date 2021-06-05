---
layout: article
title: Getting Started
description: The following post demonstrates syntax for incorporating static assets and jekyll plugins in to a blog post or page.
tags: [jekyll, jekyll theme, get started]
include-highlightjs: yes
---

### Prerequisites

Follow the [Jekyll Docs](https://jekyllrb.com/docs/installation){:target="_blank"} to complete the installation of Ruby, RubyGems, Jekyll and [Bundler](https://bundler.io){:target="_blank"}.

### Installation

At the time, this is not available via RubyGems

#### Download the Gem




#### Include

theme: jekyll-theme-perfolio

### Modify or Run Perfolio Locally

#### Get Source

Download or [Fork](https://github.com/rossgodwin/jekyll-theme-perfolio/fork){:target="_blank"} Perfolio.

#### Build Gem

This is optional but if you want to modify the code and rebuil the gem, run the following.

$ gem build jekyll-theme-perfolio

#### Run the Demo Locally

Make sure to have git installed

$ sudo apt-get install git

Change to the directory where you forked the demo.

$ bundle config set --local path 'vendor/bundle'

$ bundle install

$ bundle exec jekyll serve --config _config.yml,_config.dev.yml

Open a browser and go to the following url.

http://127.0.0.1:4000

### Demo

Visit ...

### Deploy

When you are ready to deploy
To docs folder

$ JEKYLL_ENV=production bundle exec jekyll build

