▶ [[Frenbee Document]]

---

In a [[Frenbee Document]], the term "Semantics" is used to mean usage or category in some places.

## Roles of Semantics in the Outline of a Frenbee Document

Semantics in the [[Outline]] of a [[Frenbee Document]] may be used as an [[Aspect Item]] or a [[Frenbee Animation]], as described below.

The values of Semantics are stored in the [[CSV]] format in XML representation.

### Semantics of an Aspect Item

Semantics of an [[Aspect Item]] are information that indicates which part of the aspect (body part, cloth, or accessory) of a [[Frenbee Avatar]] is represented by the [[Partial Model]] or which [[Avatar Setting]] (color or morph value) is used. If more than one part is involved, multiple parts are enumerated.

> Example: Semantics of a dress (one-piece garment) are `tops` and `bottoms`.

This way, when a change is applied to an [[Aspect Item]] from a certain [[Avatar Aspect]] (appearance state) during [[Avatar Creation]] (feature or cloth change), the resulting behavior is determined.

* An [[Avatar Aspect]] is represented as a list of [[Aspect Item]]s.
* Note that, in principle, there should be no overlap of Semantics among the items (valid state).
* Before a new [[Aspect Item]] is applied, all old [[Aspect Item]]s whose Semantics partially match (collide) are removed.
* The state of the new [[Avatar Aspect]] is completed for each individual part, based on the [[Default Aspect]] for the current [[Gender]], so that its appearance is appropriate.

### Semantics of a Frenbee Animation

In the Semantics of a [[Frenbee Animation]], set the words that categorize the usage of the animation. Currently, set the same words for the [[Machine Keywords]] as well.

## Semantics whose usage is defined

|Semantics|Description|
|---|---|
|`background`|Background. It represents a background asset.|
|`bangles`|Bracelet or wrist watch|
|`body`|Avatar's body|
|`bottoms`|Bottoms of a dress, clothes worn on the lower body, pants, or skirt|
|`cheek color`|Cheek color|
|`Close`|Animation. Closing part of the dance. End of the dance|
|`Dress`|Animation. Wait for change of clothes|
|`earrings`|Earrings|
|`ears`|Ear (shape) |
|`eyebrows`|Eyebrows|
|`eyelash color`|Eyelash color|
|`eyes`|Eye (shape) |
|`eyeshadow color`|Eye shadow color|
|`face`|Face (shape) |
|`glasses`|Glasses|
|`hair`|Hair (hair style)|
|`head`|Head (shape) |
|`lip`|Lip (size)|
|`lip color`|Lip color|
|`Move`|Animation. Move during the dance|
|`None`|Animation. Other|
|`nose`|Nose (shape) |
|`Open`|Animation. Start of the dance|
|`Prepare`|Animation. Preparation for the dance|
|`shoes`|Shoes or boots|
|`skin color`|Skin color|
|`Standby`|Animation. Preparation for the dance|
|`Step`|Animation. Move during the dance|
|`tops`|Tops of a dress, clothes worn on the upper body, jacket, or shirt|
|`Translate`|Animation. Move during the dance|

