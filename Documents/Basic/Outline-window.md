The Outline window refers to 'F.Outline', which is a window for editing the [[Outline]] information of a [[Frenbee Document]] in [[Frenbee Repository]]. This window can be used for purposes such as the following:

* Editing an [[Outline]]
* Creating a [[Folder]]
* Creating a [[Remover]]

## Opening Outline window

Open from the Main Menu ☰ `Frenbee`/`Window`/`Outline`.

Or, select the `.fren` file of a [[Frenbee Document]] in [[Frenbee Repository]] in the `Project` window and open it from the context menu ☰ `Frenbee`/`Repository`/`Edit outline`.

## Outline of F.Outline

In the `F.Outline` window, you can edit [[Outline]]s of the `.fren` files of [[Frenbee Document]]s inside folders in [[Frenbee Repository]]. Open the Outline window and select the `.fren` files of [[Frenbee Document]]s in the folders in [[Frenbee Repository]] in the `Project` window to view or edit the files.

### How to save the editing status

Edited [[Frenbee Document]]s are saved using any of the following operations, and [[Frenbee Asset Build]] processing is also performed for saved items.

* Click `Save` button explicitly.
* Switch the item selection in the `Project` window.
* Close the `F.Outline` window.

### How to discard the editing status

To cancel changes, restore the editing status or click the `Load` button explicitly.

## Operations

When the target [[Frenbee Document]] is selected, the following items are displayed and can be edited.

### Thumbnail image related items

When the [[Frenbee Document]] contains a [[Thumbnail Image]], the image is displayed. Width x Height [px] and the Gamma value are also displayed.
When the [[Frenbee Document]] does not contain a [[Thumbnail Image]], the "No image" help box is displayed.

|GUI|Description|
|---|---|
|`Import...` button|Specifies an external `.png` image file in a dialog box and imports it as a [[Thumbnail Image]]. In principle, finish processing of the image in advance, as the image is not processed at this time. A [[Thumbnail Image]] is embedded in the [[Frenbee Document]] in a special format. After importing, there is no dependency relationship between the imported image and the original image. |
|`Remove` button|Removes the [[Thumbnail Image]]. |

### Outline related items
|GUI|Description|
|---|---|
|Id|Shows the [[Id]]. (view only)|
|Version|Shows version. (view only)|
|Last Updated|Shows the [[DateTime]] of the last update data (UTC) of the file. (view only)|
|Name|Reference: Name of the [[Outline]]|
|Order|Reference:  Order of the [[Outline]]|
|Gender|Reference:  [[Gender]]|
|Semantics|Reference:  [[Semantics]]|
|`Normalize Semantics` button (displayed only when effective)|Removes whitespace characters before and after each keyword of [[Semantics]]. Removes empty or duplicate keywords and performs sorting as well. This is a function that supports input. Do not use this button when you want to include whitespaces before and after keywords or empty keywords intentionally. |
|Machine Keywords|Reference:  [[Machine Keywords]]. Enter in the [[CSV text field]] format. |
|`Normalize MKs` button (displayed only when effective)|Removes whitespace characters before and after each keyword of [[Machine Keywords]]. Removes empty or duplicate keywords and performs sorting as well. This is a function that supports input. Do not use this button when you want to include whitespaces before and after keywords or empty keywords intentionally. |
|`Fix gender in MKs` button (displayed only when effective)|Corrects [[Machine Keywords]] related to [[Gender]]. This button and a warning are displayed only when there is a problem in the relationship between [[Gender]] and [[Machine Keywords]]. |
|Search Keywords|Reference:  [[Machine Keywords]]. Enter in the [[CSV text field]] format. |
|`Normalize SKs` button (displayed only when effective)|Removes whitespace characters before and after each keyword of [[Search Keywords]]. Removes empty or duplicate keywords and performs sorting as well. This is a function that supports input. Do not use this button when you want to include whitespaces before and after keywords or empty keywords intentionally. |
|`This is a folder` checkbox|When this checkbox is ☑ (checked), the selected [[Frenbee Document]] functions as a [[Folder]]. |
|+ Machine Keywords|Reference:  The "Including Machine Keywords" condition of the [[Folder]]. Enter in the [[CSV text field]] format. |
|- Machine Keywords|Reference:  The "Excluding Machine Keywords" condition of the [[Folder]]. Enter in the [[CSV text field]] format. |
|+ Search Keywords|Reference:  The "Including Machine Keywords" condition of the [[Folder]]. Enter in the [[CSV text field]] format. |
|- Search Keywords|Reference:  The "Excluding Machine Keywords" condition of the [[Folder]]. Enter in the [[CSV text field]] format. |

### General items

|GUI|Description|
|---|---|
|`Save` button|Click this button when you want to explicitly save the editing results immediately. [[Frenbee Asset Build]] is also performed for the item. |
|`Load` button|Click this button when you want to cancel the editing results. The file will be reloaded. |
