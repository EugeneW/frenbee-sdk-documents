▶ [[Frenbee Document]]

---

An Id is information stored in a [[Frenbee Document]] to identify each individual [[Frenbee Document]] in that [[Frenbee Document]]. It is represented using a GUID ([`System.Guid`](http://docs.go-mono.com/?link=T%3aSystem.Guid) structure). In principle, the information called the Id uses the same type in relation to the [[Frenbee]] system.

## How to identify multiple Frenbee Documents

When multiple [[Frenbee Document]]s are handled in [[Frenbee Paged Assets]] or other cases, the Id stored in each [[Frenbee Document]] is used to identify the files.

* When creating a new [[Frenbee Document]] to be distinguished from other items, it is important to set a unique Id. A different [[Frenbee Document]] file with the same Id is regarded as another version of the same item.
* [`Guid.Empty`](http://docs.go-mono.com/?link=F%3aSystem.Guid.Empty) (`00000000-0000-0000-0000-000000000000`) means the item is not set or empty. (For a valid item, set a value other than this.)

> This Id is irrelevant to the GUID management of Unity assets ([`UnityEditor.AssetDatabase`](http://docs.unity3d.com/Documentation/ScriptReference/AssetDatabase.html)). (The Id space is different.)