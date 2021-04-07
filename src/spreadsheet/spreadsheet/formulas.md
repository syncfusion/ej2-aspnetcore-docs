---
title: "Formulas"
component: "Spreadsheet"
description: "This section helps you to understand the formula feature in the Essential JS 2 spreadsheet."
---

# Formulas

Formulas are used for calculating the data in a worksheet. You can refer the cell reference from same sheet or from different sheets.

## Usage

You can set formula for a cell in the following ways,

* Using the `formula` property from `cell`, you can set the formula or expression to each cell at initial load.
* Set the formula or expression through data binding.
* You can set formula for a cell by [`editing`](./editing).
* Using the [`updateCell`](../api/spreadsheet/#updatecell) method, you can set or update the cell formula.

## User Defined Functions

The list of formulas supported in the spreadsheet is sufficient for most of your calculations. If not, you can add your own custom function using the [`addCustomFunction`](../api/spreadsheet/#addcustomfunction) method. Use [`computeExpression`](../api/spreadsheet/#computeexpression) method, if you want to compute any formula or expression.

The following code example shows the calculation of data using supported and custom `formulas` in the spreadsheet.

{% aspTab template="spreadsheet/formula", sourceFiles="formulaController.cs" %}

{% endaspTab %}

## Formula bar

Formula bar is used to edit or enter cell data in much easier way. By default, the formula bar is enabled in the spreadsheet. Use the [`showFormulaBar`](../api/spreadsheet/#showformulabar) property to enable or disable the formula bar.

## Named Ranges

You can define a meaningful name for a cell range and use it in the formula for calculation. It makes your formula much easier to understand and maintain. You can add named ranges to the Spreadsheet in the following ways,

* Using the [`definedNames`](../api/spreadsheet/#definednames) collection, you can add multiple named ranges at initial load.
* Use the [`addDefinedName`](../api/spreadsheet/#adddefinedname) method to add a named range dynamically.
* You can remove an added named range dynamically using the [`removeDefinedName`](../api/spreadsheet/#removedefinedname) method.
* Select the range of cells, and then enter the name for the selected range in the name box.

The following code example shows the usage of named ranges support.

{% aspTab template="spreadsheet/defined-names", sourceFiles="definedNameController.cs" %}

{% endaspTab %}

## Supported Formulas

The following are the list of formulas supported in spreadsheet,

| Formula | Description |
|-------|---------|
| ABS | Returns the value of a number without its sign. |
| AND | Returns TRUE if all the arguments are TRUE, otherwise returns FALSE. |
| AVERAGE | Calculates average for the series of numbers and/or cells excluding text. |
| AVERAGEA | Calculates the average for the cells evaluating TRUE as 1, text and FALSE as 0. |
| AVERAGEIF | Clears content of the active cell and enables edit mode. |
| AVERAGEIFS | Calculates average for the cells based on specified conditions. |
| CEILING | Rounds a number up to the nearest multiple of a given factor. |
| CHOOSE | Returns a value from list of values, based on index number. |
| CONCAT | Concatenates a list or a range of text strings. |
| CONCATENATE | Combines two or more strings together. |
| COUNT | Counts the cells that contain numeric values in a range. |
| COUNTA | Counts the cells that contains values in a range. |
| COUNTIF | Counts the cells based on specified condition. |
| COUNTIFS | Counts the cells based on specified conditions. |
| DATE | Returns the date based on given year, month, and day. |
| DAY | Returns the day from the given date. |
| DAYS | Returns the number of days between two dates. |
| EXP | Returns e raised to the power of the given number. |
| FIND | Returns the position of a string within another string, which is case sensitive.|
| FLOOR | Rounds a number down to the nearest multiple of a given factor. |
| IF | Returns value based on the given expression. |
| IFERROR | Returns value if no error found else it will return specified value. |
| IFS | Returns value based on the given multiple expressions. |
| INDEX | Returns a value of the cell in a given range based on row and column number. |
| INT | Rounds a number down to the nearest integer. |
| INTERCEPT | Calculates the point of the Y-intercept line via linear regression. |
| ISNUMBER | Returns true when the value parses as a numeric value. |
| LN | Returns the natural logarithm of a number. |
| LOG | Returns the logarithm of a number to the base that you specify. |
| MATCH | Returns the relative position of a specified value in given range. |
| MAX | Returns the largest number of the given arguments. |
| MIN | Returns the smallest number of the given arguments. |
| OR | Returns TRUE if any of the arguments are TRUE, otherwise returns FALSE. |
| POWER | Returns the result of a number raised to power. |
| PRODUCT | Multiplies a series of numbers and/or cells. |
| RADIANS | Converts degrees into radians. |
| RAND | Returns a random number between 0 and 1. |
| RANDBETWEEN | Returns a random integer based on specified values. |
| ROUND | Rounds a number to the specified number of digits. |
| ROUNDUP | Rounds a number up, away from zero. |
| SLOPE | Returns the slope of the line from linear regression of the data points. |
| SORT | Sorts the contents of a column, range, or array in ascending or descending order. |
| SUBTOTAL | Returns subtotal for a range using the given function number. |
| SUM | Adds a series of numbers and/or cells. |
| SUMIF | Adds the cells based on specified condition. |
| SUMIFS | Adds the cells based on specified conditions. |
| SUMPRODUCT | Returns the sum of the products of the corresponding array in given arrays. |
| TEXT | Converts the supplied value into text by using the user-specified format. |
| TODAY | Returns the current date. |
| TRUNC | Truncates a supplied number to a specified number of decimal places. |

## See Also

* [Editing](./editing)
* [Formatting](./formatting)
* [Open](./open)
* [Save](./save)
