---
title: " RangeNavigator Period Selector | ASP.NET MVC "

component: "RangeNavigator"

description: "The period selector allows to select a range with specified periods."
---

# Period selector

The period selector allows to select a range with specified periods.

## Periods

Periods is an array of objects that allows users to specify the range of periods. The “interval” property specifies the count value of the button, and the “text” property specifies the text to be displayed on button. The “intervalType” property allows users to customize the intervals of the buttons. The “intervalType” property supports the following interval types:

* Auto
* Years
* Quarter
* Months
* Weeks
* Days
* Hours
* Minutes
* Seconds

{% aspTab template="range-navigator/period/periods", sourceFiles="periods.cs" %}

{% endaspTab %}

## Positioning period selector

The “position” property allows users to position the period selector either at the “top” or “bottom”.

{% aspTab template="range-navigator/period/position", sourceFiles="position.cs" %}

{% endaspTab %}

## Height

The “height” property allows users to specify the height for period selector. The default value of the height property is 43.

{% aspTab template="range-navigator/period/height", sourceFiles="height.cs" %}

{% endaspTab %}

## Visibility of range navigator

The “disableRangeSelector” property allows users to render the period selector without range navigator.

{% aspTab template="range-navigator/period/visible", sourceFiles="visible.cs" %}

{% endaspTab %}

## See Also

* [LightWeight](./light-weight/)