---
title: "Binding data to Kanban"
component: "Kanban"
description: "This section includes the data binding topics explaining how to bind various data sources to Kanban using DataManager adaptors."
---

# Data binding

The Kanban uses `DataManager`, which supports both RESTful data service binding and list binding. The `dataSource`property of Kanban can be assigned either with the instance of `DataManager` or List, as it supports the following two data binding methods:

* Local data
* Remote data

## Local data

To bind local list data to the Kanban, you can simply assign a list to the `dataSource` property. The list can also be provided as an instance of `DataManager` and assigned to the Kanban `dataSource` property.

{% aspTab template="kanban/data-binding/local-data", sourceFiles="controller.cs,datasource.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/local-data.PNG)

> By default, `DataManager` uses `JsonAdaptor` for binding local data.

## Remote data

To bind remote data to kanban component, assign service data as an instance of `DataManager` to the `dataSource`property. To interact with remote data source,  provide the endpoint **url**.

{% aspTab template="kanban/data-binding/remote-data", sourceFiles="controller.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/remote-data.PNG)

> By default, `DataManager` uses **ODataAdaptor** for remote data-binding.

### OData services

[`OData`](http://www.odata.org/documentation/odata-version-3-0/) is a standardized protocol for creating and consuming data. You can retrieve data from OData service using the DataManager. Refer to the following code example for remote Data binding using OData service.

{% aspTab template="kanban/data-binding/odata-service", sourceFiles="controller.cs" %}

{% endaspTab %}

### OData v4 services

The ODataV4 is an improved version of OData protocols, and the `DataManager` can also retrieve and consume OData v4 services. For more details on OData v4 services, refer to the [`OData Documentation`](http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part1-protocol/odata-v4.0-errata03-os-part1-protocol-complete.html#_Toc453752197). To bind OData v4 service, use the **ODataV4Adaptor**.

{% aspTab template="kanban/data-binding/odata-service", sourceFiles="controller.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/odata-v4.PNG)

### Web API

You can use **WebApiAdaptor** to bind kanban with Web API created using OData endpoint.

{% aspTab template="kanban/data-binding/web-api", sourceFiles="controller.cs" %}

{% endaspTab %}

Below server-side controller code to get the Kanban data.

```typescript

[HttpGet]
        public object Get()
        {
            var data = OrdersDetails.GetAllRecords().ToList();
            return data;
        }

```

### URL adaptor

The CRUD (Create, Read, Update and Delete) actions can be performed easily on Kanban cards using the various adaptors available within the `DataManager`. Most preferably, we will be using `UrlAdaptor` for performing CRUD actions on Kanban.

{% aspTab template="kanban/data-binding/url-adaptor", sourceFiles="controller.cs" %}

{% endaspTab %}

The server-side controller code to handle the CRUD operations are as follows.

```typescript

private NORTHWNDEntities db = new NORTHWNDEntities();
public ActionResult DataSource() {
    var DataSource = db.Tasks.ToList();
    return Json(DataSource, JsonRequestBehavior.AllowGet);
}
public ActionResult UpdateData(EditParams param) {
    if (param.action == "insert" || (param.action == "batch" && param.added != null)) {
        //Insert record in database
    }
    if (param.action == "update" || (param.action == "batch" && param.changed != null)) {
        //Update record in database
    }
    if (param.action == "remove" || (param.action == "batch" && param.deleted != null)) {
        //Delete record in database
    }
    db.SaveChanges();
    var data = db.Tasks.ToList();
    return Json(data, JsonRequestBehavior.AllowGet);
}

public class EditParams {
    public string key { get; set; }
    public string action { get; set; }
    public List<Tasks> added { get; set; }
    public List<Tasks> changed { get; set; }
    public List<Tasks> deleted { get; set; }
    public Tasks value { get; set; }
}
```

### Custom adaptor

It is possible to create your own custom adaptor by extending the built-in available adaptors. The following example demonstrates the custom adaptor usage and how to add a custom field `TaskId` for the cards by overriding the built-in response processing using the `processResponse` method of the `ODataAdaptor`.

{% aspTab template="kanban/data-binding/custom-adaptor", sourceFiles="controller.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/custom-adaptor.PNG)

### Sending additional parameters to the server

To add a custom parameter to the data request, use the **addParams** method of **Query** class. Assign the **Query** object with additional parameters to the kanban `query` property.

{% aspTab template="kanban/data-binding/additional-parameter", sourceFiles="controller.cs" %}

{% endaspTab %}

> The parameters added using the `Query` property will be sent along with the data request for every kanban action.

### Handling HTTP error

During server interaction from the kanban, some server-side exceptions may occur, and you can acquire those error messages or exception details
in client-side using the `actionFailure` event.

The argument passed to the `actionFailure` event contains the error details returned from the server.

{% aspTab template="kanban/data-binding/http-error", sourceFiles="controller.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/http-error.PNG)

> The `actionFailure` event will be triggered not only for the server errors, but
also when there is an exception while processing the kanban actions.

## Loading data via ajax

You can use Kanban `dataSource` property to bind the datasource to Kanban from external ajax request. In the following code, we have fetched the datasource from the server using ajax request and provided that to the `dataSource` property by using the **OnSuccess** event of ajax.

{% aspTab template="kanban/data-binding/data-via-ajax", sourceFiles="controller.cs" %}

{% endaspTab %}

Output be like the below.

![kanban](./images/ajax-data.PNG)

> * If you bind the DataSource from this way, then it acts like a local dataSource. So you cannot perform any server-side crud actions.
