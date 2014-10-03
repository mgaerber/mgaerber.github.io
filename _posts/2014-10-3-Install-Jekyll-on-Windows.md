---
layout: post
title: Install Jekyll on Windows
---

## 7 Steps

* Fork + clone the example Jekyll site from https://github.com/barryclark/jekyll-now (don't forget to rename the repo to yourgithubname.github.io)
* Go to http://rubyinstaller.org/downloads/ and download the RubyInstaller + DevKit
* Test your installation by entering ruby -help on the command line, then install 'Bundler' by typing 
```
  gem install bundler
```

* Run the RubyInstaller, also unzip the DevKit to some convenient location (don't forget to set PATH to include DevKit's bin and mingw/bin directories)
* Create a file called 'Gemfile' in your forked repo and put two lines there:

```
    source 'https://rubygems.org'
```   
 <br/>
```
    gem 'github-pages'
```

* Open the cmd prompt, change dir to your forked repo and enter: 
```
    bundle install
```

* Finally, to run the site locally type
```
    jekyll serve --watch
```