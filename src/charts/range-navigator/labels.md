---
title: " RangeNavigator Labels | ASP.NET MVC "

component: "RangeNavigator"

description: "RangeNavigator supports Multilevel label and enable grouping properties to customize axis labels."
---

# Labels

## Multilevel labels

The second level labels for the range navigator can be enabled by setting the “enableGrouping” property to true.
This is restricted to date-time axis alone.

{% aspTab template="range-navigator/label/multi", sourceFiles="multi.cs" %}

{% endaspTab %}

## Grouping

The second level axis labels can be grouped using “groupBy” property with the following interval types:

* Auto
* Years
* Quarter
* Months
* Weeks
* Days
* Hours
* Minutes
* Seconds

{% aspTab template="range-navigator/label/group", sourceFiles="group.cs" %}

{% endaspTab %}

## Smart labels

The “labelIntersectAction” property is used to avoid overlapping of labels.

The following code sample shows setting the labelIntersectAction property to Hide.

{% aspTab template="range-navigator/label/smart", sourceFiles="smart.cs" %}

{% endaspTab %}

## Label positioning

By default, the labels can be placed at outside of the range navigator. You can place the labels inside the range navigator
using the labelPosition property.

{% aspTab template="range-navigator/label/position", sourceFiles="position.cs" %}

{% endaspTab %}

## Labels customization

The font size, color, family, etc. can be customized using the “labelStyle” property.

{% aspTab template="range-navigator/label/custom", sourceFiles="custom.cs" %}

{% endaspTab %}