---
title: "Aggregates"
component: "TreeGrid"
description: "Learn how to aggregate rows, apply custom aggregates, and format the aggregate values in the TreeGrid control."
---

# Aggregates

Aggregate values are displayed in the TreeGrid footer and in parent row footer for child row aggregate values. It can be configured through [`e-treegrid-aggregates`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregates.html) property.
 The [`field`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Field.html) and [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html)
 are the minimum properties of [`e-treegrid-aggregate-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn.html) required to represent an aggregate column.

By default, the aggregate value can be displayed in the treegrid footer, and footer of child rows. To show the aggregate value in one of the cells, use the [`footerTemplate`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~FooterTemplate.html) property of [`e-treegrid-aggregate-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn.html) tag helper.

## Built-in aggregate types

The aggregate type should be specified in the [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html) property to configure an aggregate column.

The built-in aggregates are,
* Sum
* Average
* Min
* Max
* Count
* Truecount
* Falsecount

> Multiple aggregates can be used for an aggregate column by setting the [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html) property
with an array of aggregate types.
> Multiple types for a column is supported only when one of the aggregate templates is used.

## Footer aggregate

Footer aggregate value is calculated for all the rows, and it is displayed in the footer cells. Use the [`footerTemplate`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~FooterTemplate.html) property of [`e-treegrid-aggregate-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn.html) tag helper to render the aggregate value in footer cells.

{% aspTab template="tree-grid/aggregates/footer-aggregate", sourceFiles="footerAggregate.cs" %}

{% endaspTab %}

> The aggregate values must be accessed inside the template using their corresponding [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html) name.

## Child aggregate

Aggregate value is calculated for child rows, and it is displayed in the parent row footer. Use the [`showChildSummary`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregate~ShowChildSummary.html) property to render the child rows aggregate value.

{% aspTab template="tree-grid/aggregates/child-aggregate", sourceFiles="childAggregate.cs" %}

{% endaspTab %}

## How to format aggregate value

You can format the aggregate value result by using the [`format`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html) property of [`e-treegrid-aggregate-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn.html) tag helper.

{% aspTab template="tree-grid/aggregates/format-Aggregate", sourceFiles="formatAggregate.cs" %}

{% endaspTab %}

## Custom aggregate

To calculate the aggregate value with your own aggregate functions, use the custom aggregate option. To use custom aggregation, specify the [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~Type.html) as **Custom**, and provide the custom aggregate function in the [`customAggregate`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridAggregateColumn~CustomAggregate.html) property.

{% aspTab template="tree-grid/aggregates/custom-Aggregate", sourceFiles="customAggregate.cs" %}

{% endaspTab %}

> To access the custom aggregate value inside the template, use the key as **Custom**.