Frenbee Paged Assets is the runtime asset format for the Frenbee system. It defines the configurations of the files and folders generated by processing [[Frenbee Document]] files and the file format to be used in the storage included in the package.

> Frenbee Paged Assets is the format of assets in [[Frenbee Repository]] after they are processed by [[Frenbee Asset Build]].

* In principle, Frenbee Paged Assets is located in the `Assets/StreamingAssets/Frenbee/paged_assets` file path in a Unity project.
  * On Windows, this folder has hidden attribute. Note that you cannot browse in `Project` window of Unity. However, this will be contain a built game package.

> `StreamingAssets` is a folder name that has a special effect in Unity.  
> ☞ http://docs.unity3d.com/Documentation/Manual/StreamingAssets.html

The status of this folder can be easily checked on the [[Assets Window]].

## Format Outline

* A placement format suitable for storage systems in which there is an upper limit on the size of a single file.
* Large files will be divided so as to fit in storage systems in which there is an upper limit on the size of a single file. This is called "Paged".
* A file in the [[Document Registry]] format `registry.xml` is placed for each asset folder.
* A cache file is provided for [[Thumbnail Image]]s to simplify access. Only when the item has a [[Thumbnail Image]], a single (unnumbered) file `thumbnail` is placed.

> See ☞ [[Standard Asset Folders]] for standard folder names.
