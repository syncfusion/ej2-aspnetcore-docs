---
title: "List-box Getting started"
component: "ListBox"
description: "This section explains how to create a simple Syncfusion ASP.NET CORE list box control and configure it's functionalities."
---

# Getting Started

> Starting with v16.2.0.x, if you reference Syncfusion assemblies from trial setup or from the NuGet feed, you also have to include a license key in your projects. Please refer to this [link](https://help.syncfusion.com/common/essential-studio/licensing/license-key) to know about registering Syncfusion license key in your ASP.NET CORE application to use our components.

This section briefly explains how to include simple ListBox control in your ASP.NET Core application. You can refer to [ASP.NET Core Getting Started documentation](../getting-started/) page for system requirements, and configure common specifications.

## Adding component to the Application

* Add the ListBox component in view page to render our Syncfusion components.

{% aspTab template="listbox/getting-started/default", sourceFiles="data.cs" %}

{% endaspTab %}

## Binding data source

After initialization, populate the ListBox with data using the [`dataSource`](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2~Syncfusion.EJ2.DropDowns.ListBox~DataSource.html) property.
Here, an array of string values is passed to the ListBox component.

The following example illustrates the output in your browser.

{% aspTab template="listbox/getting-started/data", sourceFiles="data.cs" %}

{% endaspTab %}
