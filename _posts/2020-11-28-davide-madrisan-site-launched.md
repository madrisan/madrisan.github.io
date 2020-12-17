---
layout: post
category: projects
date: 2020-11-28
highcharts: on
language: en
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

##### MathJax

I can optionally enable the [MathJax](https://www.mathjax.org/) JavaScript display engine
when I need to render beautiful $$\TeX$$-formatted mathematical expressions.
For instance my preferred identity:
<div>
$$
e^{i \pi} = -1
$$
</div>

##### Highcharts

Or use the SVG-based, multi-platform charting library [Highcharts](https://www.highcharts.com/demo)
for plotting great dynamic charts.

<div id="montly-average-temperature" style="min-width: 310px; height: 400px; margin: 0 auto"></div>

<script type="text/javascript">
    $('#montly-average-temperature').highcharts({
        title: {
            text: 'Monthly Average Temperature',
            x: -20 //center
        },
        subtitle: {
            text: 'Source: WorldClimate.com',
            x: -20
        },
        xAxis: {
            categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
                'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
        },
        yAxis: {
            title: {
                text: 'Temperature (°C)'
            },
            plotLines: [{
                value: 0,
                width: 1,
                color: '#808080'
            }]
        },
        tooltip: {
            valueSuffix: '°C'
        },
        legend: {
            layout: 'vertical',
            align: 'right',
            verticalAlign: 'middle',
            borderWidth: 0
        },
        series: [{
            name: 'Tokyo',
            data: [7.0, 6.9, 9.5, 14.5, 18.2, 21.5, 25.2, 26.5, 23.3, 18.3, 13.9, 9.6]
        }, {
            name: 'New York',
            data: [-0.2, 0.8, 5.7, 11.3, 17.0, 22.0, 24.8, 24.1, 20.1, 14.1, 8.6, 2.5]
        }, {
            name: 'Berlin',
            data: [-0.9, 0.6, 3.5, 8.4, 13.5, 17.0, 18.6, 17.9, 14.3, 9.0, 3.9, 1.0]
        }, {
            name: 'London',
            data: [3.9, 4.2, 5.7, 8.5, 11.9, 15.2, 17.0, 16.6, 14.2, 10.3, 6.6, 4.8]
        }]
    });
</script>

<hr>
Hosted with :heart: by [GitHub](https://github.com/madrisan/madrisan.github.io)
