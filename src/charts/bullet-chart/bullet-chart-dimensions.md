---
title: " Bullet Chart Appearance | ASP.NET CORE "

component: "Bullet Chart"

description: "We can set bullet-chart size manually by using width and height properties. We can set percentage or pixel size values to the bullet-chart."
---

# Bullet Chart Dimensions

## Size for Container

The bullet chart can be rendered to its container’s size. You can set the size using inline or CSS as shown below.

{% aspTab template="bullet-chart/bullet-chart-dimensions/container", sourceFiles="container.cs" %}

{% endaspTab %}

## Size for Bullet Chart

You can also set the size for bullet chart directly using the [`width`](../api/bullet-chart/#width-string) and [`height`](../api/bullet-chart/#height-string) properties.

### In Pixel

You can set the size of a chart in pixels as shown below.

{% aspTab template="bullet-chart/bullet-chart-dimensions/pixel", sourceFiles="pixel.cs" %}

{% endaspTab %}

### In Percentage

By setting a value in percentage, the bullet chart gets its dimension with respect to its container. For example, when the height is ‘50%’, the bullet chart renders to half of the container’s height.

{% aspTab template="bullet-chart/bullet-chart-dimensions/percentage", sourceFiles="percentage.cs" %}

{% endaspTab %}

>Note: When you do not specify the size, it takes `126px` as its height and window size as its width.