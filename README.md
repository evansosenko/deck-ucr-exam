# Jekyll & deck.js

[![Dependency Status](https://gemnasium.com/razor-x/jekyll-and-deck.js.png)](https://gemnasium.com/razor-x/jekyll-and-deck.js)
[![Build Status](https://travis-ci.org/razor-x/jekyll-and-deck.js.png?branch=master)](https://travis-ci.org/razor-x/jekyll-and-deck.js)
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/razor-x/jekyll-and-deck.js/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

Source for your deck blog running on Jekyll and deck.js.
Just clone and deck.

- Create your [deck.js](http://imakewebthings.com/deck.js/) deck with [Jekyll](http://jekyllrb.com/).
- Asset pipeline with [Jekyll::AssetsPlugin](https://github.com/ixti/jekyll-assets).
- Bower for asset dependency management.
- Basic [Rake](https://github.com/jimweirich/rake) tasks with support for dev and testing modes, run `rake -D` for info.
- Meta data system for SEO.
- [Google Analytics](http://www.google.com/analytics/) ready: see `google_analytics` variable in `_config.yml`.
- [Piwik](https://piwik.org/) ready: set `piwik: yoursite.com/piwik/` in `_config.yml` (yoursite.com/piwik/ points to the piwik install root).

## Quick start

Just clone this with

    git clone https://github.com/razor-x/jekyll-and-deck.js.git my_blog

run `bundle && bower install` and make your deck in `index.haml`.
Head over to the [Jekyll Docs](http://jekyllrb.com/docs/home/) and [deck.js docs](http://imakewebthings.com/deck.js/docs/) for the rest of the details.

## Add future update support

If you want to merge in future updates from this project and have your own origin,
set up a separate branch to track this.

    git remote rename origin razorx-jekyll-and-deck.js
    git branch jekyll-and-deck.js
    git branch -u razorx-jekyll-and-deck.js/master jekyll-and-deck.js

Then add an origin and push master

    git remote add origin git@github.com:username/username-deck.git
    git push -u origin master

Now, the `razorx-jekyll-and-deck.js` branch will pull changes from this project,
which you can then merge into your other branches.

## Updating

The `Gemfile` is using pessimistic version constraints for everything,
so if you want major updates, you need to bump the versions yourself.

JavaScript library versions need to be updated in `bower.json` and `_config.yml`.

## License

This code is licensed under the MIT license.

## Warranty

This software is provided "as is" and without any express or
implied warranties, including, without limitation, the implied
warranties of merchantibility and fitness for a particular
purpose.
