---
title: "Resize images before uploading it to the server"
component: "Uploader"
description: "Covers customizable features of the file upload control such as a preview image, invisible upload, progress bar, sort the file list and more."
---

# Resize images before uploading it to the server

You can customize the dimension of the images before uploading it to the server.
By using selected event, you can get the selected file information as type of an object. From the obtained image file information, create a new canvas and render an image with the custom dimensions. Refer the corresponding code snippet as follows.

{% aspTab template="uploader/pre-resize", sourceFiles="pre-resize.cs,index.css" %}

{% endaspTab %}