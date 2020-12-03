---
title: " RangeNavigator Customization | ASP.NET MVC "

component: "RangeNavigator"

description: "Range navigator can be customized using the navigatorBorder, navigatorStyleSettings, seleced or unselected region color properties."
---

# Customization

## Navigator appearance

The navigator can be customized using the “navigatorStyleSettings” property. The “selectedRegionColor” property is used
to specify the color for selected region whereas the “unSelectedRegionColor” property is used to specify the color for
unselected region.

{% aspTab template="range-navigator/custom/appearance", sourceFiles="appearance.cs" %}

{% endaspTab %}

## Thumb

The thumb property provides options to customize the border, fill, size, and type of thumb. The types of thumb can be “Circle” and “Rectangle”.

{% aspTab template="range-navigator/custom/thumb", sourceFiles="thumb.cs" %}

{% endaspTab %}

## Border customization

Using the “navigatorBorder” property, you can customize the “width” and “color” of the range navigator.

{% aspTab template="range-navigator/custom/border", sourceFiles="border.cs" %}

{% endaspTab %}

## Deferred update

If the “enableDeferredUpdate” property is set to true, then the changed event will be fired after dragging the slider.
If the “enableDeferredUpdate” is false, then the changed event will be fired when dragging the slider. By default,
the “enableDeferredUpdate” is set to false.

{% aspTab template="range-navigator/custom/defer", sourceFiles="defer.cs" %}

{% endaspTab %}

## Allow snapping

The “allowSnapping” property toggles the placement of the slider exactly to the left or on the nearest interval.

{% aspTab template="range-navigator/custom/snap", sourceFiles="snap.cs" %}

{% endaspTab %}

## Animation

The speed of the animation can be controlled using the “animationDuration” property. The default value of the “animationDuration” property is 500 milliseconds.

{% aspTab template="range-navigator/custom/animation", sourceFiles="animation.cs" %}

{% endaspTab %}

## See Also

* [Grid and Tick Lines](./grid-tick/)
* [Labels](./labels/)