---
title: "Data Binding"
component: "Spreadsheet"
description: "Learn how to bind local and remote data in the Essential JS 2 Spreadsheet control."
---

# Data Binding

The Spreadsheet uses [`DataManager`](../data), which supports both RESTful JSON data services and local JavaScript object array binding to a range. The `dataSource` property can be assigned either with the instance of [`DataManager`](../data) or JavaScript object array collection.

> To bind data to a cell, use `cell data binding` support.

## Local data

To bind local data to the Spreadsheet, you can assign a JavaScript object array to the `dataSource` property.

Refer to the following code example for local data binding.

{% aspTab template="spreadsheet/local-data-binding", sourceFiles="localDataController.cs" %}

{% endaspTab %}

> The local data source can also be provided as an instance of the [`DataManager`](../data). By default, [`DataManager`](../data) uses [`JsonAdaptor`](../data/adaptors/#json-adaptor) for local data-binding.

## Remote data

To bind remote data to the Spreadsheet control, assign service data as an instance of [`DataManager`](../data) to the `dataSource` property. To interact with remote data source, provide the service endpoint `url`.

Refer to the following code example for remote data binding.

{% aspTab template="spreadsheet/remote-data-binding", sourceFiles="remoteDataController.cs" %}

{% endaspTab %}

> By default, `DataManager` uses **ODataAdaptor** for remote data-binding.

## Cell data binding

The Spreadsheet control can bind the data to individual cell in a sheet . To achive this you can use the
`value` property.

Refer to the following code example for cell data binding.

{% aspTab template="spreadsheet/cell-data-binding", sourceFiles="cellDataController.cs" %}

{% endaspTab %}

> The cell data binding also supports formula, style, number format, and more.

## See Also

* [Filtering](./filter)
* [Sorting](./sort)
* [Hyperlink](./link)
* [`Collaborative Editing`](use-cases/collaborative-editing)