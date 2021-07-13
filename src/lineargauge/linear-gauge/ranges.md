---
title: " Ranges in ASP.NET Core Linear Gauge component | Syncfusion "

component: "Linear Gauge"

description: "Learn here all about the Ranges feature of Syncfusion ASP.NET Core Linear Gauge component and more."
---

# Ranges in ASP.NET Core Linear Gauge

Range is the set of values in the axis. The range can be defined using the [`Start`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_Start) and [`End`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_End) properties in the [`e-lineargauge-range`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html). Any number of ranges can be added to the Linear Gauge using the [`e-lineargauge-ranges`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRanges.html).

{% aspTab template="lineargauge/ranges/ranges", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with ranges](../images/range.png)

## Customizing the range

Ranges can be customized using the following properties in [`e-lineargauge-range`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRanges.html).

* [`StartWidth`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_StartWidth) - To set the thickness of the range at the start axis value.
* [`EndWidth`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_EndWidth) - To set the thickness of the range at the end axis value.
* [`Color`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_Color) - To set the color of the range.
* [`Position`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_Position) - To place the range. By default, the range is placed outside of the axis. To change the position, this property can be set as "[**Inside**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.Position.html#Syncfusion_EJ2_LinearGauge_Position_Inside)", "[**Outside**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.Position.html#Syncfusion_EJ2_LinearGauge_Position_Outside)", "[**Cross**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.Position.html#Syncfusion_EJ2_LinearGauge_Position_Cross)", or "[**Auto**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.Position.html#Syncfusion_EJ2_LinearGauge_Position_Auto)".
* [`Offset`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_Offset) - To place the range with the specified distance from the axis.
* [`Border`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRange_Border) - To set the color and width for the border of the range.

{% aspTab template="lineargauge/ranges/range-customization", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with range customization](../images/range-custom.png)

## Setting the range color for the labels

To set the color of the labels like the range color, set the [`UseRangeColor`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLabel.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLabel_UseRangeColor) property as "**true**" in the [`labelStyle`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLabel.html).

{% aspTab template="lineargauge/ranges/range-labelcolor", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with range color as label color](../images/range-labelcolor.png)

## Multiple ranges

Multiple ranges can be added to the Linear Gauge by adding multiple [`e-lineargauge-range`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRange.html) objects in the [`e-lineargauge-ranges`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRanges.html) and customization for the ranges can be done with [`e-lineargauge-range`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRanges.html) object.

{% aspTab template="lineargauge/ranges/multiple-ranges", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with multiple ranges](../images/multiple-ranges.png)

## Gradient Color

Gradient support allows the addition of multiple colors in the range of the Linear Gauge. The following gradient types are supported in the Linear Gauge.

* Linear Gradient
* Radial Gradient

### Linear Gradient

Using linear-gradient, colors will be applied in a linear progression. The start value of the linear gradient can be set using the [`StartValue`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLinearGradient_StartValue) property. The end value of the linear gradient will be set using the [`EndValue`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLinearGradient_EndValue) property. The color stop values such as [`Color`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Color), [`Opacity`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Opacity), and [`Offset`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Offset) are set using [`ColorStop`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLinearGradient_ColorStop) property. The linear gradient can be rendered for the range in the Linear Gauge by using the below example.

{% aspTab template="lineargauge/ranges/lineargradient", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with linear gradient range](../images/linear-range.png)

## Radial Gradient

Using radial gradient, colors will be applied in circular progression. The inner circle position of the radial gradient will be set using the [`InnerPosition`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRadialGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRadialGradient_InnerPosition) property. The outer circle position of the radial gradient can be set using the [`OuterPosition`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRadialGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRadialGradient_OuterPosition) property. The color stop values such as [`Color`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Color), [`Opacity`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Opacity), and [`Offset`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeColorStop.html#Syncfusion_EJ2_LinearGauge_LinearGaugeColorStop_Offset) are set using [`ColorStop`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeRadialGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeRadialGradient_ColorStop) property. The radial gradient can be rendered for the range in the Linear Gauge by using the below example.

{% aspTab template="lineargauge/ranges/radialgradient", sourceFiles="" %}

{% endaspTab %}

![Linear Gauge with radial gradient range](../images/radial-range.png)

> Note: If we set both gradients for the range, only the linear gradient gets rendered. If we set the [`StartValue`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLinearGradient_StartValue) and [`EndValue`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html#Syncfusion_EJ2_LinearGauge_LinearGaugeLinearGradient_EndValue) of the [`LinearGradient`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.LinearGauge.LinearGaugeLinearGradient.html) as empty strings, then the radial gradient gets rendered in the range of the Linear Gauge.