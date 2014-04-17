`F.Outline Replacer` window is an editing utility that collectively replaces the [[Outline]] information in specific [[Frenbee Document]]s in [[Frenbee Repository]]. In other words, it is a function to replace [[Outline]] of the following target files with [[Outline]] of the source file. The relationship is identified based on the major file names of both the target files and the source file.

> Individual [[Outline]] can be edited in the [[Outline window]].

## Target file

Specific [[Frenbee Document]]s in [[Frenbee Repository]].

## Source file

The source information is the file in the [[Document Registry]] format `registry.xml` used in [[Frenbee Repository]]. This file has a file name corresponding to each item.

> On the other hand, `registry.xml` in [[Frenbee Paged Assets]] does not have a file name. This file is invalid.

## Usage examples

Outline Replacer window is effective in the following cases, for example.

### Reassembling many custom items

1. You have created multiple items.
2. You have set [[Outline]] for each of them.
3. After doing so, you need to modify the model data of a custom item.
4. You want to reassemble the custom item by using the previous [[Outline]] information.

In such a case, you can use the [[Outline]] information of the previous items through the following steps:

1. Save the `registry.xml` of [[Frenbee Repository]] to another location before making changes.
2. Re-create updated custom [[Frenbee Document]]s without changing the file names. (conversion from other formats, etc.).
3. Place these [[Frenbee Document]]s in [[Frenbee Repository]] and complete the import.
3. By applying the `registry.xml` of the previous items to these [[Frenbee Document]]s using Outline Replacer, you can restore the [[Outline]] information with ease.

## Opening Outline Replacer window

Open the `F.Outline Replacer` window from the Main Menu ☰ `Frenbee`/`Repository`/`Outline Replacer`.

## Operations

|GUI|Description|
|---|---|
|`Open...` button|Opens the XML file that will become the source file. Specify the XML file in the dialog box. The file format valid here is `registry.xml`, which is the [[Document Registry]] format used in [[Frenbee Repository]]. When a valid source file is specified here, the Outline information will be saved to the memory and the preparation for the replacement processing will be complete. |
|Valid items with file name (displayed only when the source file is valid)|The number of valid items with file names in the source file. Since replacement is performed based on file names; items without file names have no significance in the Outline Replacer window. |
|Total items (displayed only when the source file is valid)|The total number of items inside the source file|
|Replacement options|You can specify which Outline information is replaced by using the toggles displayed underneath. |
|`Overwrite (Trial)` button|Performs trial replacement processing. Only generates a file comparison log, without actually overwriting the file. |
|`Overwrite...` button|Executes replacement. Starts actual replacement processing when the `Overwrite...` button in the confirmation dialog box is clicked. The processing can be canceled by clicking the `Cancel` button on the progress bar; however, the processed files cannot be restored. After processing is complete, [[Frenbee Paged Assets]] are updated by [[Frenbee Asset Build]]. A file comparison log is also generated. |
|`Save...` button (displayed only when a log exists)| Saves the generated log as an HTML file. This HTML file contains the recorded results of the processing performed using the `Overwrite (Trial)` or `Overwrite...` buttons. It is a comparison of the Outline information between the matched Source item and Target items. Information without differences is shown in blue. Information with differences is shown in red. |
|`Save and Open...` button (displayed only when a log exists)|Opens the saved HTML file in the default method of the OS, in addition to the operation performed by the `Save` button. Generally, the file is opened with an Internet browser. |

## File name match condition

Only the major file names of [[Frenbee Document]]s in [[Frenbee Repository]] and the source file are the target of comparison. Folder names or extensions are not the comparison targets.

Outline Replacer does not consider folder hierarchies. Therefore, it is strongly recommended that the major file names be unique for all items. When there are collisions between file names, the first file name found during processing will become the processing target. At this time, no warning will be issued.

## Replacement of Outline

The [[Outline]] information of items that satisfy the file name match condition and of the source file is compared according to the conditions specified in the Replacement options. When using the `Overwrite...` button, [[Frenbee Document]]s in [[Frenbee Repository]] with differences are replaced.

