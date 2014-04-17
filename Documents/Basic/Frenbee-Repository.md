Frenbee Repository refers to the storage for editing and managing `.fren` files of [[Frenbee Document]]s.

## Frenbee Repository in Unity Project

* The following folder path is used in Unity projects in particular:  `Assets/Frenbee/Repository`
* This folder is a source folder for [[Frenbee Asset Build]] processing. [[Frenbee Document]] files in this folder path become the targets of conversion to [[Frenbee Paged Assets]].
* This folder is the target of viewing or editing in the [[Outline window]].
* Sub-folders in this folder will become the child folders of [[Frenbee Paged Assets]] with the same names after [[Frenbee Asset Build]] processing. These folder names are related to execution of the package as well. Use the default names `aspect`, `animation`, or `background`, or name each file with caution.
* All sub-sub-folders (folder hierarchy within a sub-folder) are simply flattened and placed in the sub-folders of [[Frenbee Paged Assets]]. Sub-sub-folders can be utilized only for file classification during editing/managing files.
* Since [[Frenbee Document]]s are distinguished by [[Id]], the [[Frenbee Document]]s file name here is arbitrary in principle. The file name extension is `.fren`. In principle, file names of [[Frenbee Document]]s here and file names of [[Frenbee Paged Assets]] converted by [[Frenbee Asset Build]] are unrelated. However, it is safe to choose file names that are not easily affected by each development platform. In some case, [[Id]] is the major file name.

> Since the sub-folders in Frenbee Repository are related to [[Frenbee Paged Assets]], as described above, the same rules for [[Standard Asset Folders]] can be applied to them.
