---
title: "BulletChart Tooltip | ASP.NET CORE "

component: "BulletChart"

description: "Tooltip is used to show the data value when mouse hover on the chart.We can able to customize format,template and appearance."
---

# Tooltip

BulletChart will display details about the actual and target values through tooltip, when the mouse is moved over the target and feature bar.

## Default Tooltip

By setting [`enable`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html)property to true. By default tooltip is visible in bullet-chart.

{% aspTab template="bullet-chart/tool-tip/tool-tip", sourceFiles="tool-tip.cs" %}

{% endaspTab %}

## Tooltip Template

Any HTML elements can be displayed in the tooltip by using the `template` property of the tooltip. You can use the ${target} and ${value} as place holders in the HTML element to display the value and target values of the corresponding data point.

## Customize the Appearance of Tooltip

The [`fill`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html) and [`border`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html) properties are used to customize the background color and border of the tooltip respectively. The [`textStyle`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html) property in the tooltip is used to customize the font of the tooltip text.