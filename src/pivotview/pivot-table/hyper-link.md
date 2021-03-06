---
title: "Hyperlink"
component: "Pivot Table"
description: "User allows to show hyperlink option to the link data for individual cells."
---

# Hyperlink

The pivot table supports to show hyperlink option to link data for individual cells that are displayed in the component. Also, the hyperlink can be enabled separately for row headers, column headers, value cells, and summary cells using the [`e-hyperlinkSettings`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html) tag. It can be configured through code behind, during initial rendering and the settings available to show hyperlink are:

* [`showHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowHyperlink): It allows to set the visibility of hyperlink in all cells.
* [`showRowHeaderHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowRowHeaderHyperlink): It allows to set the visibility of hyperlink in row headers.
* [`showColumnHeaderHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowColumnHeaderHyperlink): It allows to set the visibility of hyperlink in column headers.
* [`showValueCellHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowValueCellHyperlink): It allows to set the visibility of hyperlink in value cells.
* [`showSummaryCellHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowSummaryCellHyperlink): It allows to set the visibility of hyperlink in summary cells.
* [`headerText`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_HeaderText): It allows to set the visibility of hyperlink based on header text.
* [`conditionalSettings`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html): It allows to set the visibility of hyperlink based on specific condition.

<!-- markdownlint-disable MD028 -->
> By default, the hyperlink options are disabled for all cells in the pivot table.

> User defined style can be applied to hyperlink using [`cssClass`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_CssClass) property in [`e-yperlinkSettings`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html) tag.

## Hyperlink for all cells

The pivot table has an option to show hyperlink option for all cells that are currently in display. To do so, user need to set [`showHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowHyperlink) to **true**.

{% aspTab template="pivot-table/hyper-link/all-cells", sourceFiles="AllCells.cs" %}

{% endaspTab %}

![output](images/hyperlink.png)

## Hyperlink for row headers

The pivot table has an option to show hyperlink option for row header cells alone that are currently in display. To do so, user need to set [`showRowHeaderHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowRowHeaderHyperlink) to **true**.

{% aspTab template="pivot-table/hyper-link/row-header", sourceFiles="RowHeader.cs" %}

{% endaspTab %}

![output](images/hyperlink-rowheader.png)

## Hyperlink for column headers

The pivot table has an option to show hyperlink option for column header cells alone that are currently in display. To do so, user need to set [`showColumnHeaderHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowColumnHeaderHyperlink) to **true**.

{% aspTab template="pivot-table/hyper-link/column-header", sourceFiles="ColumnHeader.cs" %}

{% endaspTab %}

![output](images/hyperlink-columnheader.png)

## Hyperlink for value cells

The pivot table has an option to show hyperlink option for value cells alone that are currently in display. To do so, user need to set [`showValueCellHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowValueCellHyperlink) to **true**.

{% aspTab template="pivot-table/hyper-link/value-cells", sourceFiles="ValueCells.cs" %}

{% endaspTab %}

![output](images/hyperlink-value.png)

## Hyperlink for summary cells

The pivot table has an option to show hyperlink option for summary cells alone that are currently in display. To do so, user need to set [`showSummaryCellHyperlink`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_ShowSummaryCellHyperlink) to **true**.

{% aspTab template="pivot-table/hyper-link/summary-cells", sourceFiles="SummaryCells.cs" %}

{% endaspTab %}

![output](images/hyperlink-summary.png)

## Condition based hyperlink

The pivot table has an option to show hyperlink in the cells based on specific conditions. It can be configured using the [`conditionalSettings`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html) tag through code behind, during initial rendering. The settings required are:

* [`measure`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html#Syncfusion_EJ2_PivotView_PivotViewConditionalSetting_Measure): Specifies the value field name, in-order to set the visibility of hyperlink for the same when condition is met.
* [`conditions`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html#Syncfusion_EJ2_PivotView_PivotViewConditionalSetting_Conditions): Specifies the operator type such as [**Equals**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.Condition.html), [**GreaterThan**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.Condition.html), [**LessThan**](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.Condition.html), etc.
* [`value1`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html#Syncfusion_EJ2_PivotView_PivotViewConditionalSetting_Value1): Specifies the start value.
* [`value2`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewConditionalSetting.html#Syncfusion_EJ2_PivotView_PivotViewConditionalSetting_Value2): Specifies the end value.

{% aspTab template="pivot-table/hyper-link/conditions", sourceFiles="Conditions.cs" %}

{% endaspTab %}

![output](images/hyperlink-condition.png)

## Header based hyperlink

The pivot table has an option to show hyperlink in the cells based on specific row or column header. It can be configured using the [`headerText`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotViewHyperlinkSettings.html#Syncfusion_EJ2_PivotView_PivotViewHyperlinkSettings_HeaderText) option through code behind, during initial rendering.

{% aspTab template="pivot-table/hyper-link/headers", sourceFiles="Headers.cs" %}

{% endaspTab %}

![output](images/hyperlink-header.png)

## Event

The event [`hyperlinkCellClick`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.PivotView.PivotView.html#Syncfusion_EJ2_PivotView_PivotView_HyperlinkCellClick) fires on every hyperlink cell click.

It has following parameters - `cancel` and `currentCell`. The parameter `currentCell` is used to customize the host cell element by any means. Meanwhile, when the parameter `cancel` is set to **true**, applied customization will not be updated to the host cell element.

{% aspTab template="pivot-table/hyper-link/event", sourceFiles="Event.cs" %}

{% endaspTab %}

## See Also

* [Apply condition based hyperlink for specific row or column](./how-to/apply-condition-based-hyper-link-for-specific-row-or-column)