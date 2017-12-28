## Jasper2

[![Build Status](https://travis-ci.org/myJekyll/jasper2.svg?branch=master)](https://travis-ci.org/myJekyll/jasper2)
[![Ruby](https://img.shields.io/badge/ruby-2.4.2-blue.svg?style=flat)](http://travis-ci.org/myJekyll/jasper2)
[![Jekyll](https://img.shields.io/badge/jekyll-3.6.2-blue.svg?style=flat)](http://travis-ci.org/myJekyll/jasper2)

This is a full-featured port of Ghost's default theme from [Fábio Madeira](https://github.com/myJekyll/jasper2). See  [Casper](https://github.com/tryghost/casper)
*v2.1.7* for [Jekyll](https://jekyllrb.com/) / [GitHub Pages](https://pages.github.com/).

## Live Demo

[Ghost's Casper](https://demo.ghost.io) // [Jasper2](https://myJekyll.github.io/jasper2)

![home page](https://raw.githubusercontent.com/myJekyll/jasper2/master/assets/screenshot-desktop.jpg)


## Features

* Out of the box support for multiple authors (via `_data/authors.yml`)
* Full author information including: picture, bio, website, twitter, facebook, etc.
* Tag description(s) and personalised covers (via `_data/tags.yml`)
* Related posts view at the bottom of each post
* All Ghost default pages: Author page(s), Tag page(s), About page(s), 404, etc.
* Pagination (infinite scrolling or standard pagination, i.e. posts across multiple pages)
* Atom Feeds by [Jekyll-feed](https://github.com/jekyll/jekyll-feed)
* Toggleable subscribe button (requires an external service)
* Code Syntax Highlight with [highlight.js](https://highlightjs.org/)
* Support for Google Analytics tracking
* Support for Disqus comments (not Ghost standard)


## Getting Started

### Deployment

**Important:**  For security reasons, Github does not allow plugins (under `_plugins/`) when
deploying with Github Pages. This means:

- we need to generate your site locally (more details below) and push the resulting HTML (the contents of `_site/`) to a Github repository, that GitHub Pages then host;


- for this option simply clone this repository (*master branch*), and then run
`bundle exec jekyll serve` inside the directory. Upload the resulting `_site/` contents to your repository (*master branch* if uploading as your personal page
(e.g. username.github.io) or *gh-pages branch* if uploading as a project page
(as for the [demo](https://github.com/myJekyll/jasper2/tree/gh-pages)).


### Author Pages

In order to properly generate author pages you need to rename the field *author* in the
front matter of every post to match that of your each author's *username* as defined
in the *[\_data/authors.yml](_data/authors.yml)* file.
With the latest update, multiple author blogs are now supported out of the box.

### Compiling Styles

Following on the way Casper styles are compiled as [described here](https://github.com/tryghost/casper#development):

Jasper2 styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need Node and Gulp installed globally. After that, from the theme's root directory:

```bash
$ npm install
$ gulp
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

## Issues and Contributing

This install builds well with Ruby v2.4.2 and Jekyll v3.6.2. If you run into any problems
please log them on the [issue tracker](https://github.com/myJekyll/jasper2/issues).

Feel free pull-request your patches and fixes.

## Thanks


Many thanks to the Ghost team for all the design work. Also many thanks to all contributors,
that help keeping the project alive and updated :smile:


## Copyright & License

Same licence as the one provided by Ghost's team. See Casper's theme [license](GHOST.txt).

Copyright (C) 2015-2017 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.