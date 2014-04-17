▶ [[Frenbee Document]]

---

A Folder refers to the functions and set of information described below used to provide a virtual folder structure of the search query (filter) type to an item, Closet, etc. in a [[Frenbee Document]]. This set of information is also used as the `Item` element attributes of the [[Document Registry]].

## Function overview

1. A Folder item executes its specific search query for the entire item set to which it belongs.
2. The items that match the condition are enumerated (in an item list) as the contents that are virtually included in the folder at that point of time.
3. The default or specified sort is applied to the item list (or omitted when unnecessary).

> In C# code, the FolderQuery class corresponds to a Folder.

|Name|XML attribute/property name|Type|Description|
|---|---|---|---|
|Folder Keywords|`FolderKeywords`|[[CSV]]|Search query that "includes" [[Machine Keywords]]. A [[Frenbee Document]] matches when all specified keywords are in [[Machine Keywords]]. The matching items are considered to virtually belong to this folder and enumerated as items in the folder.| 
|Folder Excluding Machine Keywords|`FolderExcludingKeywords`|[[CSV]]|Search query that "excludes" [[Machine Keywords]]. Items including specified keywords are excluded. An item that matches any of the specified keywords is considered not to virtually belong to this folder and not enumerated as an item in the folder.| 
|Folder Including Search Keywords|`FolderSearchKeywords`|[[CSV]]|Search query that "includes" [[Search Keywords]]. A [[Frenbee Document]] matches when all specified keywords are in Keywords. The matching items are considered to virtually belong to this folder and enumerated as items in the folder.| 
|Folder Excluding Search Keywords|`FolderExcludingSearchKeywords`|[[CSV]]|Search query that "excludes" [[Search Keywords]]. Items including specified keywords are excluded. An item that matches any of the specified keywords is considered not to virtually belong to this folder and not enumerated as an item in the folder.| 
|Folder|`Folder`|Boolean|Indicates whether an item is a folder or not. When this value is `True`, the item is a folder (a query is executed). When the value is `False` (default), the item is not a folder.| 

## Characteristics of a folder item

* When `Folder` is `True`, a [[Frenbee Document]] is handled as a folder item.
* In a folder-supported system, a folder item determines the item configuration of the folder by executing a query as a virtual "folder".
* A [[Thumbnail Image]] in the Image list functions as a GUI icon, as an ordinary item does.

* A Folder is of the query search type.
 * Therefore, circular reference and self-reference are possible. 
 * A folder or item may belong to multiple folders, as in tagging. 
* It can also be used for a tree hierarchy (as with actual folders in general storages). 
 * In that case, set a specific relationship between the query and keywords so that the folder does not enumerate itself or the child-level folders and items.
* In principle, a [[Frenbee Document]] has one set of folder information.

## Base folder

* The folder that serves as the virtual base is named "Base".
* `base folder` is included in [[Machine Keywords]].
* The Base folder is intended for developers.
* Normally, the Home folder described later is handled as a child folder of the Base folder. In principle, the Base folder is set to include `home` and `folder` in Including Machine Keywords.
* To use a folder as the default Base folder, include `default` in [[Machine Keywords]]. (Currently, no specific usage of this folder is defined.)


> In the case of the Aspect Folder described later, the Base folder is called the "Aspect base folder".

## Home folder

* The folder that serves as the virtual start point is named "Home".
* `home` is included in [[Machine Keywords]].
* In the case of the default Home folder, include `default` in [[Machine Keywords]].
 * Generally, the game GUI (In-game GUI) uses the default Home folder as the start point. This folder is visible to game players. In the standard Frenbee Assets, the [[Partial Model]] folder is set as the default Home folder.
 * In the In-game GUI, the Base folder for developers can be hidden by using the Home folder as the start point, instead of the Base folder. Items that become unnecessary in the end may be removed from the package to be distributed.

> * Browsing a folder is like browsing website pages with a web browser.
>  * The folder browsing history corresponds to the page browsing history recorded as you go from one linked page to another.
>  * The Home folder corresponds to a homepage.
 
> In the case of the Aspect Folder described later, the Home folder is called the "Aspect home folder".

## Supplement

* Generally, it is desirable to include `obsolete` in `ExcludingKeywords` in (gaming) assets. 

## Aspect folder

Here is how to use folders for the tree hierarchy GUI of [[Aspect Item]].

* Use unique keywords in [[CSV]] of [[Machine Keywords]] of each folder.
 * For example, write `eyes folder` in [[CSV]], instead of `eyes,folder`. 
 * This way, the folder level can be identified clearly. It prevents a folder from enumerating the grandchild folders that should be enumerated by its child folder. 
* To use a folder exclusively for a specific Gender, set [[Gender]] (and [[Machine Keywords]]) accordingly.

> For information about how to represent an item for "removing specific Semantics", see ☞ [[Remover]].