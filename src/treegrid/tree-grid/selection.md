---
title: "Selection"
component: "TreeGrid"
description: "Learn how to select rows and cells, use range selection, and use check box selection in the Essential JS 2 TreeGrid control."
---

# Selection

Selection provides an option to highlight a row or a cell. It can be done through simple mouse down or arrow keys. To disable selection in the TreeGrid, set the [`allowSelection`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGrid~AllowSelection.html) to false.

The treegrid supports two types of selection that can be set by using the [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~Type.html) property of [`e-treegrid-selectionsettings`] tag helper. They are:

* **Single**: The Single value is set by default, and it only allows selection of a single row or a cell.
* **Multiple**: Allows you to select multiple rows or cells.
To perform the multi-selection, press and hold CTRL key and click the desired rows or cells. To select range of rows or cells, press and hold the SHIFT key and click the rows or cells.

{% aspTab template="tree-grid/selection/selection", sourceFiles="selection.cs" %}

{% endaspTab %}

## Selection mode

The treegrid supports three types of selection mode that can be set by using
[`mode`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~Mode.html) property of [`e-treegrid-selectionsettings`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings.html). They are:

* **Row**: The Row value is set by default, and allows you to select only rows.
* **Cell**: Allows you to select only cells.
* **Both**: Allows you to select rows and cells at the same time.

{% aspTab template="tree-grid/selection/selection-mode", sourceFiles="selection-mode.cs" %}

{% endaspTab %}

## Cell selection

Cell selection can be done through simple mouse down or arrow keys (up, down, left, and right).

The treegrid supports two types of cell selection mode that can be set by using
the [`cellSelectionMode`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~CellSelectionMode.html). They are:

* **Flow**: The Flow value is set by default. The range of cells are selected between the start index and end index that includes in between cells of rows.
* **Box**: Range of cells are selected from the start and end column indexes that includes in between cells of rows within the range.

{% aspTab template="tree-grid/selection/cell-selection", sourceFiles="cell-selection.cs" %}

{% endaspTab %}

> Cell selection requires the [`mode`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~Mode.html) to be **Cell** or  **Both**, and [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~Type.html) should be **Multiple**.

## Checkbox selection

Checkbox selection provides an option to select multiple treegrid records with help of checkbox in each row.

To render the checkbox in each treegrid row, you need to use checkbox column with type as **checkbox** using the column [`type`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridColumn~Type.html) property of [`e-treegrid-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridColumn.html) tag helper.

{% aspTab template="tree-grid/selection/checkbox", sourceFiles="checkbox.cs" %}

{% endaspTab %}

> By default, selection is allowed by clicking a treegrid row or checkbox in that row. To allow selection only through checkbox, you can set the
[`checkboxOnly`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~CheckboxOnly.html) property to true.
> Selection can be persisted in all the operations using the [`persistSelection`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~PersistSelection.html) property.
For persisting selection on the treegrid, any one of the columns should be defined as a primary key using the [`isPrimaryKey`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/aspnetcore/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridColumn~IsPrimaryKey.html) property of [`e-treegrid-column`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridColumn.html) tag helper .

### Checkbox selection Mode

In checkbox selection, selection can also be done by clicking on rows. This selection provides two types of Checkbox Selection mode which can be set by using the following API,
[`checkboxMode`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~CheckboxMode.html). The modes are;

* **Default**: This is the default value of the checkboxMode. In this mode, user can select multiple rows by clicking rows one by one.
* **ResetOnRowClick**: In ResetOnRowClick mode, when user clicks on a row it will reset previously selected row. Also you can perform multiple-selection in this mode by press
and hold CTRL key and click the desired rows. To select range of rows, press and hold the SHIFT key and click the rows.

{% aspTab template="tree-grid/selection/windowslikeselection", sourceFiles="window.cs" %}

{% endaspTab %}

## Toggle selection

The Toggle selection allows to perform selection and unselection of the particular row or cell. To enable toggle selection, set [`enableToggle`](https://help.syncfusion.com/cr/cref_files/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.TreeGrid.TreeGridSelectionSettings~enabletoggle.html) property of the selectionSettings as true. If you click on the selected row or cell then it will be unselected and vice versa.

{% aspTab template="tree-grid/selection/toggleselection", sourceFiles="toggleselection.cs" %}

{% endaspTab %}

>If multi selection is enabled, then first click on any selected row (without pressing Ctrl key), it will clear the multi selection and in second click on the same row, it will be unselected.
