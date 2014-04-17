▶ [[Frenbee Document]]

---

Machine Keywords are [[CSV]] format information that determines how the system mechanically handles items and their behavior in Frenbee Avatars.
They are distinguished from [[Search Keywords]] in terms of functionality.

> It is the `Keywords` attribute in `Frenbee Document` XML representation or `Keywords` in C# code.

## Keywords whose usage is defined

|Machine Keywords|Description|
|---|---|
|animation|Indicates that the item is an animation ([[Frenbee Animation]]). Under normal use, it contains one animation.|
|aspect|Aspect model|
|background|Background model|
|bangles|Indicates the item corresponding to the bangles in [[Semantics]].|
|blank|Indicates that the item is a blank background model.|
|body|Indicates an item corresponding to the body in [[Semantics]].|
|both|Indicates that [[Gender]] is set to both (male and female). In principle, this must match the Gender attribute.|
|bottoms|Indicates an item corresponding to the bottoms in [[Semantics]].|
|cheek color|Indicates an item corresponding to the cheek color in [[Semantics]].|
|Close|
|default|Item comprising the [[Default Aspect]]|
|Dress|
|earrings|Indicates an item corresponding to the earrings in [[Semantics]].|
|ears|Indicates an item corresponding to the ears in [[Semantics]].|
|empty|Indicates a [[Remover]]. It is used to remove [[Semantics]] of the item. For example, it may be used to indicate an item for removing an accessory.|
|eyebrows|Indicates an item corresponding to the eyebrows in [[Semantics]].|
|eyelash color|Indicates an item corresponding to the eyelash color in [[Semantics]].|
|eyes|Indicates an item corresponding to the eyes in [[Semantics]].|
|eyeshadow color|Indicates an item corresponding to the eyeshadow color in [[Semantics]].|
|face|Indicates an item corresponding to the face in [[Semantics]].|
|female|Indicates that [[Gender]] is set to female. In principle, this must match the Gender attribute.|
|glasses|Indicates an item corresponding to the glasses in [[Semantics]].|
|hair|Indicates an item corresponding to the hair in [[Semantics]].|
|head|Indicates an item corresponding to the head in [[Semantics]].|
|integrated|Indicates an [[Integrated Model]].|
|lip|Indicates an item corresponding to the lip in [[Semantics]].|
|lip color|Indicates an item corresponding to the tops in [[Semantics]].|
|male|Indicates that [[Gender]] is set to male. In principle, this must match the Gender attribute.|
|Move|
|None|
|nose|Indicates an item corresponding to the nose in [[Semantics]].|
|obsolete|Obsolete item. This is used to indicate an item that is no longer used (or can no longer be used) to avoid the risk that destroying the data itself may cause a failure.|
|Open||
|Prepare||
|preset|Indicates an item bundled with the game package (*1).|
|required|Indicates an item resident in the game's memory (*1).|
|room|Indicates the background model of a room (*1).|
|shoes|Indicates an item corresponding to the shoes in [[Semantics]].|
|skin color|Indicates an item corresponding to the skin color in [[Semantics]].|
|stage|Indicates the background model of a dance stage (*1).|
|Standby||
|starter|Indicates an item that has an instance (one instance in principle) in the Closet for an initial state Frenbee Account.|
|Step||
|suits|Indicates an item that has multiple [[Semantics]] (for reference).|
|tops|Indicates an item corresponding to the tops in [[Semantics]].|
|Translate||
|unsearchable|Item that cannot be searched with [[Search Keywords]]|

## Reserved keywords

The following keywords are reserved for future use.

|Machine Keywords|Description|
|---|---|
|indisposable|Reserved. This indicates an item that is not disposable with regard to an item instance.|
|exclusive|Reserved. This indicates an item that cannot be dealt with between users with regard to an item instance.|
|ticket|Reserved. This indicates a ticket item.|

> *1: Traditional meaning for Frenbee-related products
