# blog
My blog nikokiuru.com

## Create a new project

    $ cd docs
    $ jekyll new .

## Run Jekyll with PowerShell

### Development environment

    PS $env:JEKYLL_ENV="development" ; bundle exec jekyll serve

### Production environment

    PS $env:JEKYLL_ENV="production" ; bundle exec jekyll serve

## Import data from Wordpress

Here is an introduction how to import data from your Wordpress site to Jekyll.

Let's get started with installing all dependencies:

    $ gem install jekyll-import hpricot open_uri_redirections

Export `wordpress.xml` from your Wordpress site and move it next to `import.rb`. After that run the script with Ruby:

    $ ruby import.rb

Jekyll-import will create two directories: _posts and assets.

Source: https://import.jekyllrb.com/docs/wordpressdotcom/