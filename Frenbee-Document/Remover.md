▶ [[Frenbee Document]]

---

In Frenbee, an item indicating that items that meet specified conditions should be removed from an item set is called a Remover (Remover Item). For an item to be a Remover, at least the following condition must be met:

* `empty` is included in [[Machine Keywords]].

## Aspect Remover

Particularly, when an [[Avatar Aspect]] is changed, an item for "removing an item of specific [[Semantics]]" can be represented as follows.

> In a certain GUI, the function to remove items is not available for all [[Semantics]] but limited to part of the items such as accessories. One method to provide an item removal function only for specific [[Semantics]] is by representing it as a [[Frenbee Document]].

* Such a [[Frenbee Document]] item is called a "Remover".

### Configuration and content of a Frenbee Document that is a standard Aspect Remover

* `empty` is included in [[Machine Keywords]].
* [[CSV]] of the [[Semantics]] to be removed is specified (multiple values can be specified).
* No specific content (such as the model) exists.
* A [[Thumbnail Image]] is included.

### Behavior of a Remover-enabled system

* When a Remover is applied to an [[Avatar Aspect]], the applicable [[Semantics]] are removed, not replaced or added.
