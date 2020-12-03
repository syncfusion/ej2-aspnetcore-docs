---
title: "Bullet Chart Axis Customization | ASP.NET CORE "

component: "Bullet Chart"

description: "Bullet Chart axis includes different customizations such as majortick and minortick, axis label, axis range."
---

# Axis Customization

## MajorTickLines and MinorTickLines Customization

You can customize the `width`, `color`, and `size` of minor and major tick lines using the
[`majorTickLines`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartMajorTickLines.html) and [`minorTickLines`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartMinorTickLines.html) properties of the bullet-chart.

## Tick Placement

You can place major and minor ticks `inside` or `outside` the ranges using the [`tickPosition`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.TickPosition.html) property of bullet-chart.

## Label Format

***Axis Label Format***

Axis numeric labels can be formatted by using the `labelFormat` property. Axis labels support all globalize formats. The following table describes the result of applying some commonly used label formats on numeric axis values.

{% aspTab template="bullet-chart/axis-customization/label-format", sourceFiles="label-format.cs" %}

{% endaspTab %}

The following 'Table' describes the result of applying some commonly used 'Label' formats on Numeric axis values.

<!-- markdownlint-disable MD033 -->
<table>
<tr>
<td><b>Label Value</b></td>
<td><b>Label Format property value</b></td>
<td><b>Result </b></td>
<td><b>Description </b></td>
</tr>
<tr>
<td>1000</td>
<td>n1</td>
<td>1000.0</td>
<td>The Number is rounded to 1 decimal place</td>
</tr>
<tr>
<td>1000</td>
<td>n2</td>
<td>1000.00</td>
<td>The Number is rounded to 2 decimal place</td>
</tr>
<tr>
<td>1000</td>
<td>n3</td>
<td>1000.000</td>
<td>The Number is rounded to 3 decimal place</td>
</tr>
<tr>
<td>0.01</td>
<td>p1</td>
<td>1.0%</td>
<td>The Number is converted to percentage with 1 decimal place</td>
</tr>
<tr>
<td>0.01</td>
<td>p2</td>
<td>1.00%</td>
<td>The Number is converted to percentage with 2 decimal place</td>
</tr>
<tr>
<td>0.01</td>
<td>p3</td>
<td>1.000%</td>
<td>The Number is converted to percentage with 3 decimal place</td>
</tr>
<tr>
<td>1000</td>
<td>c1</td>
<td>$1000.0</td>
<td>The Currency symbol is appended to number and number is rounded to 1 decimal place</td>
</tr>
<tr>
<td>1000</td>
<td>c2</td>
<td>$1000.00</td>
<td>The Currency symbol is appended to number and number is rounded to 2 decimal place</td>
</tr>
</table>

## GroupingSeparator

To separate groups of thousands, use the [`enableGroupSeparator`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html) property of bullet-chart.

## Custom Label Format

You can also customize the axis label format using a placeholder like ${value}K, in which the value represents the axis label, e.g. $20K.

{% aspTab template="bullet-chart/axis-customization/custom-label", sourceFiles="custom-label.cs" %}

{% endaspTab %}

## Label Placement

You can customize the axis labels `inside` or `outside` the bullet-chart using the [`labelPosition`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.LabelPosition.html) property.

## Opposed Position

To place an axis opposite to its original position,
set the [`opposedPosition`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Charts.BulletChartBuilder.html) property to true.

## Category Label

You can display the x axis label by mapping the `categoryField` from dataSource of a bullet-chart. It is a more efficient way to understand data.

{% aspTab template="bullet-chart/axis-customization/category", sourceFiles="category.cs" %}

{% endaspTab %}

## Category Label Customization

You can customize the category label by using the `categoryLabelStyle` property of the bullet-chart.

{% aspTab template="bullet-chart/axis-customization/category-label", sourceFiles="category-label.cs" %}

{% endaspTab %}