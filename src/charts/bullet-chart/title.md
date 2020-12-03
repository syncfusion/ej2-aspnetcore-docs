---
title: " Bullet Chart Title and SubTitle | ASP.NET CORE "

component: "Bullet Chart"

description: "The title and sub-title is very useful to understand the bullet chart in efficient way. It describes what kind of data which represtend by the bullet-chart. "
---

# Title

A title can be given to a bullet chart using the `title` property to show information about the data plotted.

{% aspTab template="bullet-chart/title/title", sourceFiles="title.cs" %}

{% endaspTab %}

## SubTitle

A subtitle can also be given to a bullet chart using the `subtitle` property to show additional information about the data plotted.

{% aspTab template="bullet-chart/title/sub-title", sourceFiles="sub-title.cs" %}

{% endaspTab %}

## Title and SubTitle Position

You can place the title and subtitle in different positions. By using the `titlePosition` property of the bullet chart, you can place the title and subtitles in different positions like `left`, `right`, `top`, and `bottom`.

### Position as Left

By setting the `titlePosition` to `Left`, you can display the title and subtitle at the left side of the chart.

{% aspTab template="bullet-chart/title/left", sourceFiles="left.cs" %}

{% endaspTab %}

### Position as Right

By setting the `titlePosition` to `Right`, you can display the title and subtitle at the right side of the chart.

{% aspTab template="bullet-chart/title/right", sourceFiles="right.cs" %}

{% endaspTab %}

### Position as Top

By setting the `titlePosition` to `Top`, you can display the title and subtitle at the top of the chart. The default title and subtitle positions of the bullet chart is `Top`.

{% aspTab template="bullet-chart/title/top", sourceFiles="top.cs" %}

{% endaspTab %}

### Position as Bottom

By setting the `titlePosition` to `Bottom`, you can display the title and subtitle at the bottom of the chart.

{% aspTab template="bullet-chart/title/bottom", sourceFiles="bottom.cs" %}

{% endaspTab %}

## Title Customization

You can customize the bullet chart title’s `fontStyle`, `size`, `color`, `fontWeight`, and `fontFamily` using the `titleStyle` property.

{% aspTab template="bullet-chart/title/title-custom", sourceFiles="title-custom.cs" %}

{% endaspTab %}

## SubTitle Customization

You can customize the bullet chart subtitle’s `fontStyle`, `size`, `color`, `fontWeight`, and `fontFamily` using the `subtitleStyle` property.

{% aspTab template="bullet-chart/title/sub-title-custom", sourceFiles="sub-title-custom.cs" %}

{% endaspTab %}