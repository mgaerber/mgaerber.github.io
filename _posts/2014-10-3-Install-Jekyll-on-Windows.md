---
layout: post
title: Install Jekyll on Windows
---

# 6 Steps

1. Fork + clone the example Jekyll site from https://github.com/barryclark/jekyll-now (don't forget to rename the repo to yourgithubname.github.io)
2. Go to http://rubyinstaller.org/downloads/ and download the RubyInstaller + DevKit
3. Test your installation by entering ruby -help on the command line, then install 'Bundler' by typing 

  gem install bundler

4. Run the RubyInstaller, also unzip the DevKit to some convenient location (don't forget to set PATH to include DevKit's bin and mingw/bin directories)
5. Create a file called 'Gemfile' in your forked repo and put two lines there:

  source 'https://rubygems.org'
  gem 'github-pages'

6. Open the cmd prompt, change dir to your forked repo and enter: bundle install
