---
title: "Cell"
component: "TreeGrid"
description: "Learn how to customize the TreeGrid cells with styling, text wrapping, and tooltips."
---

# Cell

## Displaying the HTML content

The HTML tags can be displayed in the TreeGrid header and content by enabling the [`disableHtmlEncode`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridColumn~DisableHtmlEncode.html) property.

{% aspTab template="tree-grid/cell/html-encode", sourceFiles="htmlEncode.cs" %}

{% endaspTab %}

## Customize cell styles

The appearance of cells can be customized by using the [`queryCellInfo`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGrid~QueryCellInfo.html) event.
The [`queryCellInfo`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGrid~QueryCellInfo.html) event triggers for every cell. In that event handler, you can get **QueryCellInfoEventArgs** that contains the details of the cell.

{% aspTab template="tree-grid/cell/query-cell", sourceFiles="queryCell.cs" %}

{% endaspTab %}

## Auto wrap

The auto wrap allows the cell content of the treegrid to wrap to the next line when it exceeds the boundary of the cell width. The Cell Content wrapping works based on the position of white space between words.
To enable auto wrap, set the [`allowTextWrap`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGrid~AllowTextWrap.html) property to **true**.

Note: When a column width is not specified, then auto wrap of columns will be adjusted with respect to the treegrid's width.

{% aspTab template="tree-grid/cell/auto-wrap", sourceFiles="autoWrap.cs" %}

{% endaspTab %}
