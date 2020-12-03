---
title: " Bullet Chart Target Bar | ASP.NET CORE "

component: "Bullet Chart"

description: "The line marker that runs perpendicular to the orientation of the graph is known as the `Comparative Measure`. "
---

# Target Bar

The line marker that runs perpendicular to the orientation of the graph is known as the `Comparative Measure` and is used as a target marker to compare against the Feature Measure value. This is also called as `Target Bar` of the bullet chart. Also, if you want to display the target bar you should map the `targetField` name from the dataSource.

{% aspTab template="bullet-chart/target-bar/target-bar", sourceFiles="target-bar.cs" %}

{% endaspTab %}

## Target Bar Types

You can customize the shape of the target bar or comparative bar using the `targetTypes` property of the bullet chart. Target bar contains `Circle`, `Cross`, and `Rect` shapes. The default type of target bar is `Rect`.

{% aspTab template="bullet-chart/target-bar/target-types", sourceFiles="target-types.cs" %}

{% endaspTab %}

## Customization

### Color Customization

Using the `targetColor` property of the bullet chart, you can customize the fill color of the target bar.

{% aspTab template="bullet-chart/target-bar/target-color", sourceFiles="target-color.cs" %}

{% endaspTab %}

### Width Customization

You can customize the width of the target bar using the `targetWidth` property of the bullet chart.

{% aspTab template="bullet-chart/target-bar/target-width", sourceFiles="target-width.cs" %}

{% endaspTab %}