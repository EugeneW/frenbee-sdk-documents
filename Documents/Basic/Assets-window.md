The Assets Window is the `F.Assets` window for editing [[Frenbee Paged Assets]] within a Unity project.
This window is related to projects using [[Frenbee Paged Assets]].

## Outline

It displays the status of [[Frenbee Paged Assets]] built by [[Frenbee Asset Build]] from [[Frenbee Repository]]. In principle, the contents visible in the `F.Assets` change by editing folders or files in [[Frenbee Repository]].

> In this window, operations in files or folders targeted by [[Frenbee Paged Assets]] within the project are performed. Exercise caution when simultaneously operating functions dependent on [[Frenbee Paged Assets]] and [[Frenbee Repository]].

## Usage

* To check status of [[Frenbee Paged Assets]].

For example, you can check the status of a [[Frenbee Document]] for a [[Frenbee Avatar]] created uniquely for a game after it is converted into [[Frenbee Paged Assets]] in [[Frenbee Repository]] by [[Frenbee Asset Build]].

## Reference

* Add [[Frenbee Document]]s for [[Frenbee Avatar]]s created uniquely for games to [[Frenbee Repository]]. They will be added to [[Frenbee Paged Assets]] by [[Frenbee Asset Build]].
* If items that are not used are deleted from [[Frenbee Repository]], the capacity of [[Frenbee Paged Assets]] will decrease. The package size of a game built in Unity can also be reduced.

## Opening the Assets Window

Opens from Main Menu ☰ `Frenbee`/`Window`/`Assets`.

## How to edit Frenbee Paged Assets

|GUI|Description|
|---|---|
|`Rebuild from Frenbee Repository` button|Executes Rebuild of [[Frenbee Asset Build]]. Same as Main Menu ☰ `Frenbee`/`Repository`/`Rebuild Assets`. |
|Asset Folders| A list of Asset Folders. In [[Frenbee Paged Assets]], items are saved in several different sub-folders according to purpose. Refer to [[Standard Asset Folders]]. Asset Folders is a list from which a sub-folder to be edited is selected. |
|Path|The file path of the selected Asset Folder can be checked. |
|`Select Folder` button|Sets the selected Asset Folder to a selected status in the `Project` window (functions only under a specific condition).|
|Paged Asset Items|A list of items registered in the selected Asset Folder. |
|`Add Frenbee Document file` button|Converts and registers [[Frenbee Document]]s. Select a file in the dialog box displayed. |
|Id|The ID of the selected item can be checked. |

## When adding a new Asset Folder

1. Create a new folder in a specified folder with Unity Editor (Context Menu ☰ `Create`/`Folder`) and set a desired name.
2. When the Asset Window is refocused, the display is updated.
3. Initialize the folder to a registerable status using the `Initialize Folder` button (above).

## When changing the Asset Folder name

1. Change the folder name with Unity Editor.
2. When the Asset Window is refocused, the display is updated.

> Refer to [[Standard Asset Folders]] for standard folder names.

## When FrenbeeAssetsEditorWindow.Editable is set to `true`

> [deprecated]

When FrenbeeAssetsEditorWindow.Editable is set to `true` in the script, the edit function will be enabled.
It is assumed that [[Frenbee Asset Build]] and [[Frenbee Repository]] are not used in this case.

|GUI|Description|
|---|---|
|`Create Frenbee Assets Folder` button (only when Frenbee Assets Folder does not exist)| Displayed when the folder for [[Frenbee Paged Assets]] does not exist. Creates the specified folder when clicked. |
|`-` button (Asset Folder)|Used to delete the entire Asset Folder. Displays a confirmation dialog box when clicked. The folder is moved to the recycle bin of the operation system by the `Delete` button (depending on the Unity behavior); however, exercise caution when performing this operation as it cannot be undone simply. |
|`-` button (Item)|Deletes an item. |
|`Initialize Folder` button (only when an uninitialized Asset Folder is selected)|Displayed when the folder content is uninitialized or broken. Empties the folder so that items can be added when clicked. |

