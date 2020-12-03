---
title: " RangeNavigator Export and Print | ASP.NET MVC "

component: "RangeNavigator"

description: "The rendered rangenavigator can be printed or exported directly from the browser by calling the public method print and export."
---

# Export and print

## Export

The rendered range navigator can be exported to JPEG, PNG, SVG, or PDF format using the export method in the range navigator. The input parameters for this method are Export Type for format and fileName for result.

{% aspTab template="range-navigator/print/export", sourceFiles="export.cs" %}

{% endaspTab %}

## Print

The rendered range navigator can be printed directly from the browser by calling the public method print. The ID of the range navigator div element must be passed as argument to that method.

{% aspTab template="range-navigator/print/print", sourceFiles="print.cs" %}

{% endaspTab %}
