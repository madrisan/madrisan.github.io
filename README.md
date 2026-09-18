madrisan.github.io
=====================

This is the code of my personal website and blog,
powered by [Jekyll](http://jekyllrb.com), the [Liquid](https://shopify.github.io/liquid/)
template language, and [kramdown](https://kramdown.gettalong.org/).
The layout is enriched by the usage of
[Bootstrap 4](https://getbootstrap.com/),
[Font Awesome](https://fontawesome.com/) and some
[Google Fonts](https://fonts.google.com/).

The site URL is https://madrisan.github.io/

## Development

### Setup (tested on Fedora, Ruby 4.0)
```
sudo dnf install rubygems ruby-devel gcc-c++

# gem cleanup (seems a good practice after a distro release upgrade)
rm -fr ~/.local/share/gem/

./script/bootstrap
```
`script/bootstrap` installs the latest `bundler`, runs `bundle install`, and works around a packaging
incompatibility between the old `sassc` gem (pinned by `jekyll-sass-converter ~> 2.1`) and modern RubyGems: `sassc`
hardcodes the path to its compiled native library relative to its own `lib/` directory, but newer RubyGems installs
native extensions into a separate per-Ruby-ABI cache directory instead, so the script symlinks it into the place
`sassc` expects. Do *not* pin an old `bundler` version manually (e.g. `gem install bundler:2.2.31`) — that version
predates a `did_you_mean` API that changed in Ruby 4.0 and crashes immediately.

### Run a local web server
```
bundle exec jekyll serve --livereload
```
Open a browser tab at `http://127.0.0.1:4000/`
