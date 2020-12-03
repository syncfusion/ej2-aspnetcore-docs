---
title: " Bullet Chart Ranges | ASP.NET CORE "

component: "Bullet Chart"

description: "Bullet Chart scale can be rendered by using different types of end values. They are used to represnt the status of each data. "
---

# Ranges

`Ranges` are represents the quality of a specific range in bullet-chart scale like good, bad and satisfactory. The `end` property specifies the ending point of the qualitative range. `Minimum` value of quantitative scale is considered as the starting point of first range and previous end points are considered as starting point for other ranges.

{% aspTab template="bullet-chart/ranges/ranges", sourceFiles="ranges.cs" %}

{% endaspTab %}

## Color Customization

Color for each qualitative range is customized using `color` property based on end values. Also you can customize the opacity of the each range color.

{% aspTab template="bullet-chart/ranges/ranges-custom", sourceFiles="ranges-custom.cs" %}

{% endaspTab %}