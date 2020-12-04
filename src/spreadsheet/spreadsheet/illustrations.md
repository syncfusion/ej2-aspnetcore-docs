---
title: "Illustrations"
component: "Spreadsheet"
description: "This section shows how to insert a image, shapes and graphic objects in the Essential JS 2 spreadsheet."
---

# Illustrations

Illustrations helps you to insert a image, shapes and graphic objects in the Essential JS 2 spreadsheet.

## Image

Adding images to a spreadsheet can enhance the visual appeal and help convey information more clearly.

> * The default value for `allowImage` property is `true`.

### Insert Image

You can insert the image by using one of the following ways,

* Selecting the Insert tab in the Ribbon toolbar, and then choose the Image tab.
* Use the `insertImage()` method programmatically.

The available parameters in `insertImage()` method are,

| Parameter | Type | Description |
|-----|------|----|
| images | `ImageModel` | Specifies the options to insert image in spreadsheet. |
| range(optional) | `string` | Specifies the range in spreadsheet. |

The available arguments in `ImageModel` are:

* src: Specifies the image source.
* id: Specifies image element id.
* height: Specifies the height of the image.
* width: Specifies the width of the image.
* top: Specifies the height of the image.
* left: Specifies the width of the image.

> * In spreadsheet, you can add many types of image files, including IMAGE, JPG, PNG, GIF and JPEG files.

### Delete Image

* If you want to delete the image, just select the image firstly, and then press the Delete key.
* Use the `deleteImage()` method programmatically.

The available parameters in `deleteImage()` method are,

| Parameter | Type | Description |
|-----|------|----|
| id | `string` | Specifies the id of the image element to be deleted. |
| range(optional) | `string` | Specifies the range in spreadsheet. |

### Image Customization

Image feature allows you to view and insert a image in a spreadsheet and you can change the height and width of the image by resizing and move it to another position.

#### Height and Width

* You can change the height and width of the image by resizing.
* Use the `height` and `width` property in the `insertImage()` method programmatically.

#### Top and Left

* You can change the position of the image by drag and drop.
* Use the `top` and `left` property in the `insertImage()` method programmatically.

{% aspTab template="spreadsheet/image", sourceFiles="imageController.cs" %}

{% endtab %}

## See Also

* [Formatting](./formatting)
* [Rows and columns](./rows-and-columns)
* [Hyperlink](./link)
* [Sorting](./sort)
