---
title: "ListView Getting Started"
component: "ListView"
description: "Getting started with ASP.NET Core ListView component."
---

# Getting Started

This section briefly explains about how to render ListView component in your ASP.NET Core application. You can refer [ASP.NET Core Getting Started documentation](../getting-started) page for introduction part of the system requirements and configure the common specifications.

> Starting with `v16.2.0.x`, if you reference Syncfusion assemblies from trial setup or from the NuGet feed, you also have to include a license key in your projects. Please refer to this [link](https://help.syncfusion.com/common/essential-studio/licensing/license-key) to know about registering Syncfusion license key in your ASP .NET Core application to use our components.

## Adding ListView component to the Application

ListView component can be rendered with the help of `ejs-listview` tag helper. Now open your view page and add the below code which initializes the ListView component.

```cs
// ListView with Empty DataSource
<ejs-listview id="list"></ejs-listview>

```

## Bind dataSource

After initialization, populate the ListView with data using the `dataSource` property. Here, the JSON values are passed to the ListView component.

```cs

public IActionResult Index()
        {
            //define the array of JSON
            List<object> data = new List<object>();
            data.Add(new { text: "Artwork", id: "01" });
            data.Add(new { text: "Abstract", id: "02" });
            data.Add(new { text: "Modern Painting", id: "03" });
            data.Add(new { text: "Ceramics", id: "04" });
            data.Add(new { text: "Animation Art", id: "05" });
            data.Add(new { text: "Oil Painting", id: "06" });
            ViewBag.dataSource = data;
            return View();
        }

```

```cs
    // ListView with DataSource
    <ejs-listview id="list" dataSource="@ViewBag.dataSource"></ejs-listview>

```

## Run the application

 After successful compilation of your application, simply press `F5` to run the application.

 The following example shows a basic ListView.

{% aspTab template="listview/getting-started/core", sourceFiles="HomeController.cs" %}

{% endaspTab %}

Output be like the below.

![ListView Sample](./images/listview.PNG)

## See Also

[Data Binding Types](./data-binding)

[ListView customization](./customizing-templates)

[Virtualization](./virtualization)