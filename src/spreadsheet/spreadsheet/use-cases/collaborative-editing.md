---
title: "Collaborative Editing in Spreadsheet"
component: "Spreadsheet"
description: "This section helps to learn how to collaborative editing in Spreadsheet control"
---

# Collaborative Editing

The collaborative editing support allows you to work at a spreadsheet collaboratively with other users. Multiple users can access to the the same spreadsheet simultaneously.

## Dependencies

The following dependent script is required to use the collaborative editing support in spreadsheet.

```js
<script src="https://cdnjs.cloudflare.com/ajax/libs/aspnet-signalr/1.1.4/signalr.js"></script>
```

## Server configuration

To make the communication between the server to the connected clients and from clients to the server, you need to configure the signalR Hubs using the following code.

```js

// For signalR Hub connection

var connection = new signalR.HubConnectionBuilder().withUrl('https://ej2services.syncfusion.com/production/web-services/hubs/spreadsheethub',{
    skipNegotiation: true,
    transport: signalR.HttpTransportType.WebSockets
  }).build();

```

## Client configuration

To broadcast the data for every action is spreadsheet, you need to transfer the data to the server through `send` method in `actionComplete` event and receive the same data by using the `dataReceived` method. In the `dataReceived` method, you need to update the action to the connected clients through `updateAction` method.

The following code example shows `Collaborative Editing` support in the Spreadsheet control.

{% aspTab template="spreadsheet/collaborative-editing", sourceFiles="collaborativeController.cs" %}

{% endaspTab %}

## Prevent the particular action update for collaborative client

Using the `action` argument from the `actionComplete` event, you can prevent the particular action update for collaborative client.

The following code example shows how to prevent collaborative client from updating the `format` action.

{% aspTab template="spreadsheet/collaborative-prevent-action", sourceFiles="collaborativePreventController.cs" %}

{% endaspTab %}