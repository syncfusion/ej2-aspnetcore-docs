---
title: "Query Builder Getting Started"
component: "Query Builder"
description: "This section helps to learn how to create the query builder in ASP.NET Core application with its basic features in step-by-step procedure."
---

# Getting Started

This section briefly explains about how to create a simple Query Builder in your ASP.NET Core application. You can refer [ASP.NET Core Getting Started documentation](../getting-started) page for introduction part of the system requirements and configure the common specifications.

## Add Query Builder to the project

To create simple Query Builder add the `ejs-querybuilder` tag with id attribute as `element` in your **Index.cshtml** page.

{% aspTab template="query-builder/getting-started/querybuilder", sourceFiles="default.cs" %}

{% endaspTab %}

## Run the application

 After successful compilation of your application, simply press `F5` to run the application.

 The following example shows a default rendering of Query Builder.

Output be like the below.

![querybuilder Sample](./images/querybuilder.png)

## Render with rule

The following example shows a basic Query Builder component with rule.

{% aspTab template="query-builder/getting-started/demo", sourceFiles="default.cs" %}

{% endaspTab %}

Output be like the below.

![querybuilder Sample](./images/querybuilder-rule.png)