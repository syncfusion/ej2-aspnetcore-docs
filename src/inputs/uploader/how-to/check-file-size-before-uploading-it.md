---
title: "Check file size before uploading"
component: "Uploader"
description: "Covers customizable features of the file upload control such as a preview image, invisible upload, progress bar, sort the file list and more."
---

# Check file size before uploading it

By using [uploading](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Inputs.Uploader.html#Syncfusion_EJ2_Inputs_Uploader_Uploading) event, you can get the file size before upload it to server.
File object contains the file size in bytes only.
You can convert the size to standard formats (`KB` or `MB`) using **bytesToSize** method.

{% aspTab template="uploader/check-file-size", sourceFiles="check-file-size.cs,index.css" %}

{% endaspTab %}