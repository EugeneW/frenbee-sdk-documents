Frenbee Asset Build is a mechanism that converts [[Frenbee Asset]]s from the [[Frenbee Repository]] format to the [[Frenbee Paged Assets]] format.

Frenbee Asset Build operates in the following manner, according to its functions or situations.

|Function|Description|
|---|---|
|When Unity recognizes an addition/update of the `Project` window (Assets folder), `Project` window Context Menu ☰: `Reimport All`, or Context Menu ☰ of the [[Frenbee Document]] `.fren` on the`Project` window:  `Reimport`|Performs Frenbee Asset Incremental Build described below for the target [[Frenbee Document]] `.fren` file. |
|Main Menu ☰ `Frenbee`/`Repository`/`Build Assets`|Frenbee Asset Incremental Build described below is performed for all [[Frenbee Document]]s. When Unity recognizes a file update, Frenbee Asset Incremental Build is performed; therefore, there is almost no need to use this explicitly. |
|Main Menu ☰ `Frenbee`/`Repository`/`Rebuild Assets`|Frenbee Asset Clean Build described below is performed for all [[Frenbee Document]]s. |
|`Project` window Context Menu ☰ `Frenbee`/`Repository`/`Create a new Frenbee Document`|You can create [[Frenbee Document]] `.fren` by using this menu in [[Frenbee Repository]]. (Tentative:  [[Id]] is a local ID that does not conflict with other IDs in [[Frenbee Repository]]. Make sure that [[Frenbee Asset]] is synchronized to avoid the possibility of a conflict in [[Frenbee Paged Assets]]. You can make the created [[Frenbee Document]] `.fren` file into an item that functions as a [[Folder]] or [[Remover]] by editing it in the [[Outline window]]. |
|When a [[Frenbee Document]] is saved in the [[Outline window]]|Frenbee Asset Incremental Build from [[Frenbee Repository]] to [[Frenbee Paged Assets]] is performed for the [[Frenbee Document]]. During this processing, no dialog box, etc., is displayed, and processing cannot be undone. |

## Frenbee Asset Incremental Build

Frenbee Asset Incremental Build is the so-called incremental build, and performs conversion from [[Frenbee Repository]] to [[Frenbee Paged Assets]].

It performs an update of or addition to each [[Frenbee Document]] `.fren` file in the target [[Frenbee Repository]] based on the information in the [[Id]], Version, and LastUpdated fields. Items in [[Frenbee Paged Assets]] that do not have a corresponding [[Id]] in [[Frenbee Repository]] disappear from [[Frenbee Paged Assets]].

A progress bar may appear during processing. In this case, processing can be canceled by the item. However, exercise caution as you cannot undo cancellation. The processing result will be displayed in a dialog box for each child folder. Check the processing details in the `Console` window.

## Frenbee Asset Clean Build

Frenbee Asset Clean Build is the so-called clean build, and performs conversion from [[Frenbee Repository]] to [[Frenbee Paged Assets]].

It adds items to all the [[Frenbee Document]] `.fren` files in [[Frenbee Repository]] by the child folder after the folder is initialized, based on the information in the [[Id]] field.

When the contents of [[Frenbee Paged Assets]] are collapsed for some reason, this Frenbee Asset Clean Build is more reliable. A progress bar appears during processing, and processing can be canceled by the item. However, exercise caution as you cannot undo cancellation. The processing result will be displayed in a dialog box for each child folder. Check the processing details in the `Console` window.
