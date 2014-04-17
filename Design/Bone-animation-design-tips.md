▶ [[Model design specifications]] ▶ Bone animation design tips

---
## Upper body

* Basically, the upper body is moved with the `ShoulderCenter` bone. To add a more detailed movement, use the `ShoulderCenter2` bone on a supplementary basis.
Note, however, that the range of movement is narrow (H: -10 to +10, P: -20 to +20, B: -10 to +10 [°]). Exercise care not to cause disruption.

![bone_a.png](bone_a.png)

## Head

* Basically, the head is moved with the `Neck` bone. The `Head` bone may be used together only when the head needs to be moved significantly. In that case, moving the `Neck` bone and `Head` bone at a ratio of 7:3 makes for a smooth head movement.

![bone_b.png](bone_b.png)