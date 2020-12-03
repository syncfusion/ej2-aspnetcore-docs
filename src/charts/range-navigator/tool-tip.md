---
title: " RangeNavigator Tooltip | ASP.NET MVC "

component: "RangeNavigator"

description: "The range navigator supports tooltips for sliders.Tooltips  display the selected start and end values."
---

# Tooltip

<!-- markdownlint-disable MD036 -->

The range navigator supports tooltips for sliders. Sliders are used to select data at a range in the range navigator.
Tooltips  display the selected start and end values.

<!-- markdownlint-disable MD013 -->

## Enable Tooltip

The tooltip is useful to show the selected data. You can enable tooltip by setting the enable property as true in tooltip object.

{% aspTab template="range-navigator/getting-started/tooltip", sourceFiles="tooltip.cs" %}

{% endaspTab %}

## Customization

Tooltips can be customized using the following properties:

* tooltip: Customizes the text displayed in tooltip.
* enable: Customizes the visibility of the tooltip.
* fill: Customizes the background color of the tooltip.
* opacity: Customizes the opacity of the tooltip.
* textStyle: Customizes the font size, color, family, style, weight, alignment, and overflow of the tooltip.

{% aspTab template="range-navigator/tooltip/tooltip", sourceFiles="tooltip.cs" %}

{% endaspTab %}

## Label Format

You can format and parse the date to all globalize format using `labelFormat` property in an axis.

{% aspTab template="range-navigator/tooltip/format", sourceFiles="format.cs" %}

{% endaspTab %}

The following table describes the result of applying some common date time formats to the `labelFormat` property

<!-- markdownlint-disable MD033 -->
<table>
<tr>
<td><b>Label Value</b></td>
<td><b>Label Format Property Value</b></td>
<td><b>Result </b></td>
<td><b>Description </b></td>
</tr>
<tr>
<td>new Date(2000, 03, 10)</td>
<td>EEEE</td>
<td>Monday</td>
<td>The Date is displayed in day format</td>
</tr>
<tr>
<td>new Date(2000, 03, 10)</td>
<td>yMd</td>
<td>04/10/2000</td>
<td>The Date is displayed in month/date/year format</td>
</tr>
<tr>
<td>new Date(2000, 03, 10)</td>
<td> MMM </td>
<td>Apr</td>
<td>The Shorthand month for the date is displayed</td>
</tr>
<tr>
<td>new Date(2000, 03, 10)</td>
<td>hm</td>
<td>12:00 AM</td>
<td>Time of the date value is displayed as label</td>
</tr>
<tr>
<td>new Date(2000, 03, 10)</td>
<td>hms</td>
<td>12:00:00 AM</td>
<td>The Label is displayed in hours:minutes:seconds format</td>
</tr>
</table>