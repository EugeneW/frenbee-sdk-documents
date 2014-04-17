## Frenbee Avatar System Overview

|||
|---|---|
|[[Model Integration]]|The Frenbee Avatar system supports dynamic appearance changes of avatars (appearance and costume change) by [[Model Integration]]. Avatar appearance can be changed with [[Avatar Aspect]]. |
|[[Bone Integration]]|You can integrate [[Additional Bones]] in a Frenbee Avatar by [[Bone Integration]]. It can be used to create a creature having bones that have been uniquely extended or a new costume, or used in combination with prebuilt items. → [[How to use additional bones]]|
|Hull system|The function to perform culling by the mesh unit. →[[Hull]]|
|[[Frenbee Animation]]|Mainly supports skeletal animation for bone movements or deformation of decorations (Skin Deformer) and morph target animation for facial expressions (Facial Animation). |

* [[Model Integration]]
 * [[Partial Model]]
 * [[Integrated Model]]
 * [[Bone Integration]]
  * [[Standard Bones]]
  * [[Additional Bones]]

## Main Components of Frenbee Avatar

If you desire to create custom avatars or items, custom animation or other custom assets using different polygon meshes, perform conversion between [[Frenbee Document]] and general purpose file formats using [[Frenbee Document Converter]], etc., and create or edit assets using an external DCC (digital content creation) software. In doing so, such a DCC software needs to be equipped with editing and input/output conversion functions supporting the following elements in principle.

* Model
 * 3D triangle mesh (Skinned mesh)
  * Vertices:  Position/Normal/Texture UV Coordinate/Bone Index/Bone Weights
 * Bones 
 * 2D Texture Images (Diffuse)
 * Materials:  Diffuse Color/Specular Color/Specular Power (Shininess)/Emissive Color/Ambient Color
 * Morphs (Blendshapes)
* Animation
 * Bone Animation
 * Morph Animation (Blendshape Animation)

>  If the editing and input/output conversion functions of the DCC do not support these elements appropriately, information will become missing or damaged, and therefore only custom assets that do not require such information can be created.
