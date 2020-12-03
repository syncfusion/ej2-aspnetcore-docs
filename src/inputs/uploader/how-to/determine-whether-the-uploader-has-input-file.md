---
title: "Determine whether the uploader has input file (required validation)"
component: "Uploader"
description: "Covers customizable features of the file upload control such as a preview image, invisible upload, progress bar, sort the file list and more."
---

# Determine whether uploader has file input (required validation)

By setting **required** attribute to uploader input element, you can validate the file input has any value in it.
In the below sample, set required attribute to the uploader input element and showcase the validation failure message using `data-required-message` attribute.

{% aspTab template="uploader/required", sourceFiles="required.cs, index.css" %}

{% endaspTab %}