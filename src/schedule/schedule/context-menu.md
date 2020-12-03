---
title: "Context Menu | ASP.Net Core Scheduler"
component: "Scheduler"
description: "This section explains how to integrate the context menu manually to a Scheduler and use it with required options."
---

# Context menu

You can display context menu on work cells and appointments of Scheduler by making use of the `ContextMenu` control manually from the application end. In the following code example, context menu control is being added from sample end and set its target as `Scheduler`.

On Scheduler cells, you can display the menu items such as `New Event`, `New Recurring Event` and `Today` option. For appointments, you can display its related options such as `Edit Event` and `Delete Event`. The default event window can be opened for appointment creation and editing using the `openEditor` method of Scheduler.

The deletion of appointments can be done by using the `deleteEvent` public method. Also, the `selectedDate` property can be used to navigate between different dates.

> You can also display custom menu options on Scheduler cells and appointments. Context menu will open on tap-hold in responsive mode.

{% aspTab template="schedule/context-menu", sourceFiles="data.cs"  %}

{% endaspTab %}