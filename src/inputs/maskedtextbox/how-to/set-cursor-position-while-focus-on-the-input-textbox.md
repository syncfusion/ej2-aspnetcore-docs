# Set cursor position while focus on the input textbox

By default, on focusing the MaskedTextBox the entire mask gets selected. You can customize by using any one of the following methods:

* Setting cursor position at the start of the MaskedTextBox.
* Setting cursor position at the end of the MaskedTextBox.
* Setting cursor at the specified position in the MaskedTextBox.

Following is an example that demonstrates the above cases to set cursor position in the MaskedTextBox using [focus](https://help.syncfusion.com/cr/aspnetcore-js2/Syncfusion.EJ2.Inputs.MaskedTextBox.html#Syncfusion_EJ2_Inputs_MaskedTextBox_Focus) event.

{% aspTab template="maskedtextbox/cursorposition", sourceFiles="cursorPosition.cs" %}

{% endaspTab %}

Output be like the below.

![MaskedTextBox Sample](../images/cursor-position.png)