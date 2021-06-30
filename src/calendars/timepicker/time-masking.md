---
title: "Time masking"
component: "TimePicker"
description: "Miscellaneous aspects of customizing the TimePicker"
---

# Enable the Masked Input

The TimePicker has built-in support to masking the time value, when `enableMask` property set as `true`.

{% aspTab template="timepicker/mask-module/mask-input", sourceFiles="" %}

{% endaspTab %}

The mask pattern is defined based on the provided time format to the component. If the format is not specified, the mask pattern is formed based on the default format of the current culture.

The selected portions of date and time co-ordinates  can  be incremented and decremented using the Up/Down arrow keys. You can also use Right/Left arrow keys to navigate from one segment to another.

The following example demonstrates default and custom format of TimePicker component with mask module.

{% aspTab template="timepicker/mask-module/mask-format", sourceFiles="date-format.cs" %}

{% endaspTab %}

# Configure Mask Placeholder

You can change mask placeholder value through property `maskPlaceholder`. By default , it takes the full name of  time co-ordinates such as `hour`, `minute` and `second`.

The following example demonstrates default and customized mask placeholder value.

{% aspTab template="timepicker/mask-module/mask-placeholder", sourceFiles="mask-placeholder.cs" %}

{% endaspTab %}
