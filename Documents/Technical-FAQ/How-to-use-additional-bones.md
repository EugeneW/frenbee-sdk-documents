You can add Bones of [[Additional Bones]] as an original game expansion in addition to Frenbee models [[Standard Bones]] provided by [[Reference Avatar Model]].  Please follow below.

## Workflow

Refer to these steps according to the purpose of editing a Bone.

* [[How to create a custom prebuilt avatar with DCC]]
* [[How to create custom items with DCC]]

## Editing Bones

Edit the added Bones using the editing process of the external DCC.

1. Add a Bone to a model.  Choose a unique name for the Bone.  The hierarchy of the Bone that [[Additional Bones]] can be added should be one the followings for the group of the Bone in the model.
 * Parentless root Bone
 * Child Bone of [[Standard Bones]]
 * Child Bone of other [[Standard Bones]]
2. Add/edit a Mesh affected by the added Bone as necessary.
3. Properly set the Bone weight of each vertex of the Mesh affected by the additional Bone.

For the details about edit, please refer to the operation manual of your DCC.

## Note for editing bones and adding bones

* As a general rule, the name of the additional Bone should not be the same as an existing one in the [[Standard Bones]].  Avoid the same name of other [[Additional Bones]] even though its purpose is different.  The bone name is referred to from bone animations.
* The number of Bone that vertex can depend on as [[Frenbee Avatar]] is maximum 4 (bone / vertex).  In Unity, it is drawn as 4 or 2 (bone / vertex) depending on Unity settings.
* The sum of vertexes independent from Bone or Bone weights should not be zero. If the sum is zero, this causes unnatural drawings such that a vertex stuck to a space.
* The [[Frenbee Avatar]] system executes [[Bone Integration]] in [[Model Integration]].  The Bones having the same name appearing in multiple [[Partial Model]] are considered as the same attribute. If you provide a Bone that does not meet this rule, it causes unexpected integration results or drawing results that are related to the integration order.
* Avoid conflict of Bone names.
* Do not modify [[Standard Bones]] carelessly.
