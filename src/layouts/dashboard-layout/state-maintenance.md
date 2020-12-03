---
title: "Panel State Maintenance"
component: "Dashboard Layout"
description: "This section explains how to save and restore the panels settings of Dashboard Layout component"
---

# Panel state maintenance

The current layout structure of the Dashboard Layout component can be obtained and saved to construct another dashboard with same panel structure using the `serialize` public method of the component. This method returns the component's current panel setting which can be used to construct a dashboard with the same layout settings.

The following sample demonstrates how to save and restore the state of the panels using the serialize method. Click Save to store the panel's settings and click Restore to restore the previously saved panel settings.

{% aspTab template="dashboard-layout/state-maintenance/", sourceFiles="HomeController.cs" %}

{% endaspTab %}

Output be like the below.

![State maintenance](./images/state_maintenance.PNG)
