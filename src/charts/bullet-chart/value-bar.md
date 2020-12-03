---
title: " Bullet Chart Value Bar | ASP.NET CORE "

component: "Bullet Chart"

description: "The main data value is encoded by a length of the main bar in the middle of the chart, known as the Feature Measure. "
---

# Feature Bar

The main data value is encoded by a length of the main bar in the middle of the chart, known as the `Feature Measure`. This is also called as `value Bar`. Also, if you want to display the target bar you should map the `valueField` name from the dataSource.

{% aspTab template="bullet-chart/value-bar/value-bar", sourceFiles="value-bar.cs" %}

{% endaspTab %}

## Feature Bar Types

You can customize the shape of the feature bar or value bar using the `type` property of the bullet chart. Feature bar contains `Rect` and `Dot` shapes. The default type of feature bar is `Rect`.

{% aspTab template="bullet-chart/value-bar/types", sourceFiles="types.cs" %}

{% endaspTab %}

## Customization

### Border Customization

Using the `valueBorder` property of the bullet chart, you can customize the border `color` and `width` of the feature bar.

{% aspTab template="bullet-chart/value-bar/value-border", sourceFiles="value-border.cs" %}

{% endaspTab %}

### Fill color and height Customization

You can customize the fill color and height of the feature bar using the `valueFill` and `valueHeight` properties of the bullet chart.

{% aspTab template="bullet-chart/value-bar/value-fill", sourceFiles="value-fill.cs" %}

{% endaspTab %}