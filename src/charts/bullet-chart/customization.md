---
title: " Bullet Chart Customization | ASP.NET CORE "

component: "Bullet Chart"

description: "Bullet Chart have different customizable features like different orientation, flow directions and animation features"
---

# Orientation

Bullet Chart can be rendered in different mode as `Horizontal` or `vertical` by using `orientation` property of the bullet-chart. By default bullet-chart rendered in horizontal mode.

{% aspTab template="bullet-chart/customization/orientation", sourceFiles="orientation.cs" %}

{% endaspTab %}

## Flow Direction

Using `enableRtl` boolean property of the bullet-chart, you can render bullet-chart in right to left or left to right direction.

{% aspTab template="bullet-chart/customization/right-to-left", sourceFiles="right-to-left.cs" %}

{% endaspTab %}

## Animation

By setting `animation` property value as `true`, you can enable the linear animation of the feature and target bars.

{% aspTab template="bullet-chart/customization/animation", sourceFiles="animation.cs" %}

{% endaspTab %}

## Theme

Bullet chart also support different types of themes. Using `theme` property of the bullet-chart, you can customize the theme styles.

{% aspTab template="bullet-chart/customization/theme", sourceFiles="theme.cs" %}

{% endaspTab %}