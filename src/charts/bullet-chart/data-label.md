---
title: " Bullet Chart Data Labels | ASP.NET CORE"

component: "Bullet Chart"

description: "Bullet Chart can be rendered by using different types of data source. They are called local data, remote data. "
---

# Data Label

Data label can be added to a bullet-chart feature bars by enabling the `enable` option in the dataLabel. By default,the labels will arrange smartly without overlapping.

{% aspTab template="bullet-chart/data-label/data-label", sourceFiles="data-label.cs" %}

{% endaspTab %}

## Customization

By using `labelStyle` property in data label, you can customize the `color`, `size` and `font`.

{% aspTab template="bullet-chart/data-label/data-label-custom", sourceFiles="data-label-custom.cs" %}

{% endaspTab %}