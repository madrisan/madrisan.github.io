---
layout: post
category: projects
date: 2020-11-28
highcharts: on
language: gb
location: Nice
mathjax: on
summary: Well. Finally got around to putting this website together...
title: My new website is born
---

Well. Finally got around to putting this website together.

Powered by [Jekyll](http://jekyllrb.com) and the [Liquid](https://shopify.github.io/liquid/)
template language and I can even use [Markdown](https://en.wikipedia.org/wiki/Markdown)
([kramdown](https://kramdown.gettalong.org/) to be precise) to author my posts
(if I'm too lazy to write in HTML).
The layout is enriched by the usage of
[Bootstrap 4](https://getbootstrap.com/), the
[Font Awsome](https://fontawesome.com/) and some
[Google Fonts](https://fonts.google.com/) too.
It actually was a lot easier than I thought it was going to be because of the
great [Jonathan McGlone's project](https://github.com/hankquinlan/hankquinlan.github.io/)
that helped me putting the main pieces toghether.

I can optionally enable the [MathJax](https://www.mathjax.org/) JavaScript display engine
when I need to render beautiful $$\TeX$$-formatted mathematical expressions.
For instance my preferred identity:

<div>
$$
e^{i \pi} = -1
$$
</div>

Or use the SVG-based, multi-platform charting library [Highcharts](https://www.highcharts.com/demo)
for plotting great dynamic charts.

<figure class="highcharts-figure">
   <div id="container-highcharts"></div>
   <p class="highcharts-description">
      This is an example of a percentage-stacked area chart picked from the official
      project documentation.
   </p>
   <script type="text/javascript"
           src="/assets/js/javascripts/blog-highcharts-000001.js"></script>
</figure>

And last but not least it's possible to make use of the [{Rouge}](http://rouge.jneen.net/)
syntax highlighter.

```html
<a href="#">Hello world</a>
```

*That's all for now, but stay tuned because other contents are coming!*

<hr>
Hosted with :heart: by [GitHub](https://github.com/madrisan/madrisan.github.io)
