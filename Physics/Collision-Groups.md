If there is penetration between the [[Collider]]s of adjacent [Rigid Bodies](Rigid Body), particularly those connected by a joint, the Rigid Bodies collide with each other (when a non-collision group is not set) and the joint attempts to suppress the movement from the collision, resulting in a violent movement.

To avoid this problem, Groups and Ignore Groups can be set for [Rigid Bodies](Rigid Body).
By using the principle described in the example below, you can nullify unnecessary collisions that may otherwise occur in joints and accessories.

Example:

1. Set Rigid Body A to Group 0 and Rigid Body B to Group 1.
2. Include 1 in Rigid Body A's Ignore Group (and/or include 0 in Rigid Body B's Ignore Group).
3. This prevents Rigid Bodies A and B from colliding with each other.