|GUI|Description|
|---|---|
|Enabled|Enabled when the box is ☑ (checked).|
|Name|Name. Name-referenced from [[Joint]].|
|Bone|Name of the target bone (GameObject)|
|Move Style|Physic: Moved with physics.<br>Kinematic: Moved with animation without the use of physics (IsKinematic of Unity/Rigidbody)|
|Groups|Sets associated collision groups (see ☞ [[Collision Groups]]). (GUI limitation: Only one group can be selected from the inspector of the FrenbeePhysics component.)|
|Ignore Groups|Sets non-collision groups (see ☞ [[Collision Groups]]). (GUI limitation: Only one group can be selected from the inspector of the FrenbeePhysics component.)|
|Mass|Mass (Set a value larger than 0.)|
|Angular Drag|Rotation drag (rotation attenuation)|
|Colliders|List of collision shapes (see ☞ [[Collider]]). If there is no shape element (Size is 0), no collision occurs. If you set multiple shapes, you can express complex collision shapes.|