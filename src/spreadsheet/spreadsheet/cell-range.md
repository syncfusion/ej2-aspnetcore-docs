---
title: "Cell Range"
component: "Spreadsheet"
description: "Learn the various operations that you can perform in range of cells of the Essential JS 2 Spreadsheet."
---

# Cell Range

A group of cells in a sheet is known as cell range.

## Wrap text

Wrap text allows you to display large content as multiple lines in a single cell. By default, the wrap text support is enabled. Use the [`allowWrap`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Spreadsheet.Spreadsheet.html#Syncfusion_EJ2_Spreadsheet_Spreadsheet_AllowWrap) property to enable or disable the wrap text support in spreadsheet.

Wrap text can be applied or removed to a cell or range of cells in the following ways,

* Using the `wrap` property in `cell`, you can enable or disable wrap text to a cell at initial load.
* Select or deselect wrap button from ribbon toolbar to apply or remove the wrap text to the selected range.
* Using the [`wrap`](../api/spreadsheet/#wrap) method, you can apply or remove the wrap text once the component is loaded.

The following code example shows the wrap text functionality in spreadsheet.

{% aspTab template="spreadsheet/wrap-text", sourceFiles="wrapTextController.cs" %}

{% endaspTab %}

### Limitations of Wrap text

The following features have some limitations in wrap text:

* Sorting with wrap text applied data.
* Merge with wrap text

## Merge cells

Merge cells allows users to span two or more cells in the same row or column into a single cell. When cells with multiple values are merged, top-left most cell data will be the data for the merged cell. By default, the merge cells option is enabled. Use [`allowMerge`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Spreadsheet.Spreadsheet.html#Syncfusion_EJ2_Spreadsheet_Spreadsheet_AllowMerge) property to enable or disable the merge cells option in spreadsheet.

You can merge the range of cells in the following ways,

* Set the `rowSpan` and `colSpan` property in `cell` to merge the number of cells at initial load.
* Select the range of cells and apply merge by selecting the desired option from ribbon toolbar.
* Use [`merge`](../api/spreadsheet/#merge) method to merge the range of cells, once the component is loaded.

The available merge options in spreadsheet are,

| Type | Action |
|-------|---------|
| Merge All | Combines all the cells in a range in to a single cell (default). |
| Merge Horizontally | Combines cells in a range as row-wise. |
| Merge Vertically | Combines cells in a range as column-wise. |
| UnMerge | Splits the merged cells into multiple cells. |

The following code example shows the merge cells operation in spreadsheet.

{% aspTab template="spreadsheet/merge-cells", sourceFiles="mergeCellController.cs" %}

{% endaspTab %}

### Limitations of Merge

The following features have some limitations in Merge:

* Merge with filter.
* Merge with wrap text.

## Data Validation

Data Validation is used to restrict the user from entering the invalid data. You can use the [`allowDataValidation`](../api/spreadsheet/#allowDataValidation) property to enable or disable data validation.

> * The default value for `allowDataValidation` property is `true`.

### Apply Validation

You can apply data validation to restrict the type of data or the values that users enter into a cell.

You can apply data validation by using one of the following ways,

* Select the Data tab in the Ribbon toolbar, and then choose the Data Validation item.
* Use the [`addDataValidation()`](../api/spreadsheet/#addDataValidation) method programmatically.

### Clear Validation

Clear validation feature is used to remove data validations from the specified ranges or the whole worksheet.

You can clear data validation rule by one of the following ways,

* Select the Data tab in the Ribbon toolbar, and then choose the Clear Validation item.
* Use the [`removeDataValidation()`](../api/spreadsheet/#removeDataValidation) method programmatically.

### Highlight Invalid Data

Highlight invalid data feature is used to highlight the previously entered invalid values.

You can highlight an invalid data by using one of the following ways,

* Select the Data tab in the Ribbon toolbar, and then choose the Highlight Invalid Data item.
* Use the [`addInvalidHighlight()`](../api/spreadsheet/#addInvalidHighlight) method programmatically.

### Clear Highlighted Invalid Data

Clear highlight feature is used to remove the highlight from invalid cells.

You can clear the highlighted invalid data by using the following ways,

* Select the Data tab in the Ribbon toolbar, and then choose the Clear Highlight item.
* Use the [`removeInvalidHighlight()`](../api/spreadsheet/#removeInvalidHighlight) method programmatically.

{% aspTab template="spreadsheet/data-validation", sourceFiles="dataValidation.cs" %}

{% endaspTab %}

### Limitations of Data validation

The following features have some limitations in Data Validation:

* Entire row data validation.
* Insert row between the data validation.
* Copy/paste with data validation.
* Delete cells between data validation applied range.

## Clear

Clear feature helps you to clear the cell contents (formulas and data), formats (including number formats, conditional formats, and borders) in a spreadsheet. When you apply clear all, both the contents and the formats will be cleared simultaneously.

### Apply Clear Feature

You can apply clear feature by using one of the following ways,

* Select the clear icon in the Ribbon toolbar under the Home Tab.
* Using the [`clear()`](../api/spreadsheet/#clear) method to clear the values.

Clear has the following types in the spreadsheet,

| Options | Uses |
|-----|------|
| `Clear All` | Used to clear all contents, formats, and hyperlinks.  |
| `Clear Formats` | Used to clear the formats (including number formats, conditional formats, and borders) in a cell. |
| `Clear Contents` | Used to clear the contents (formulas and data) in a cell. |
| `Clear Hyperlinks` | Used to clear the hyperlink in a cell. |

### Methods

Clear the cell contents and formats in the Spreadsheet document by using the [clear](../api/spreadsheet/#clear) method. The [clear](../api/spreadsheet/#clear) method has `type` and `range` as parameters. The following code example shows how to clear the cell contents and formats in the button click event.

{% aspTab template="spreadsheet/clear", sourceFiles="clearController.cs" %}

{% endaspTab %}

## See Also

* [Rows and columns](./rows-and-columns)
* [Formatting](./formatting)
* [Hyperlink](./link)
* [Sorting](./sort)
* [Filtering](./filter)
