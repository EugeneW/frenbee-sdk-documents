Avatar GameObject refers to a method having the specified GameObject hierarchies described in the following, used to make a Frenbee Avatar respond to physics.

## Hierarchical structure of Avatar GameObject

* Avatar: The name is arbitrary. Set this hierarchy to Avatar GameObject. <sup>[1]</sup>  
In this hierarchy, there is a GameObject hierarchy of each bone. Add "Rigidbody" to these bones, or add "Collilder" (collision shape) as the child GameObjects of the bones. <sup>[2]</sup>
  * Joints:  A GameObject for editing, expressing the Joint information as the Frenbee Physics by a set of child GameObjects (do not give this GameObject a hierarchical structure). When this GameObject does not exist when Physics are applied, it is automatically generated.

[1] When using the automatic physics application function by [[FrenbeeDocument component]], specify the same GameObject as that of the [[FrenbeeDocument component]]. This is the simplest way.
When personally controlling the physics application timing, it is possible to specify a different GameObject.

[2] The reason why Colliders are used as child GameObjects. This is to make it possible to express a collision shape by a composite of multiple Colliders.
