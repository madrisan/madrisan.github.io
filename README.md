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

### Setup (tested on Fedora 36)
```
sudo dnf install rubygems ruby-devel gcc-c++

# gem cleanup (seems a good practice after a distro release upgrade)
rm -fr ~/.local/share/gem/

# install most of the required gems
gem update

# then install all the missing ones (listed by the `bundle exec` command below)
#   gem install bundler:2.2.31
#   gem install sassc:2.4.0
#   ...
```

### Run a local web server
```
bundle exec jekyll serve --livereload
```
Open a browser tab at `http://127.0.0.1:4000/
