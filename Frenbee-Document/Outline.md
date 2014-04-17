▶ [[Frenbee Document]]

---

> The Outline can be edited using the [[Outline window]].

The Outline is an attribute set of `Cobitto` elements showing an outline of a [[Frenbee Document]].

> In the [[Frenbee Core]], it is the `Document` class and its properties. Part of it is stored in the `Tag` property.

It is also an attribute set of `Item` elements in the [[Document Registry]].

> In the [[Frenbee Core]], each individual item is the `DocumentLink` class and its properties.

|Name|XML attribute/property name|Type|Description|
|---|---|---|---|
|Display Name|`Name`|String|Display name. In principle, the name is displayed as it is written.|
|Order|`Order`|Int32|Interger representing the order of items. It is one of the indices that determine the display order in a sort-enabled item list. It is recommended to assign values to the initial item set in steps of 100 or at similarly large intervals, in case additional items may need to be sorted in the list later. See ☞ [[How to prioritize a custom item in a list view]]|
|[[Semantics]]|`Semantics`|[[CSV]]|String set representing the usage|See ☞ [[Semantics]]|
|[[Machine Keywords]]|`Keywords`|[[CSV]]|Keyword set for searches by humans. See ☞ [[Machine Keywords]]|
|[[Search Keywords]]|`SearchKeywords`|[[CSV]]|Keyword set for searches by humans. See ☞ [[Search Keywords]]|
|[[Gender]]|`Gender`|Gender enumeration|Enum value (`None`, `Male`, `Female`, or `Both`) of the Gender of a Frenbee Avatar that can add this item to an Aspect. See ☞ [[Gender]]|
|[[Folder]]|`Folder`|Boolean|Boolean value (`True` or `False`) indicating whether the item is a folder or not. If True, this item functions as a folder, in which case the [[Folder]]-related attributes are used.|
|Name Visible|`NameVisible`|Boolean|Boolean value indicating whether the name is visible on the In-game GUI. If True, the name is visible.|
|Last Updated|`LastUpdated`|[[DateTime]]|Value indicating the last updated date and time|
