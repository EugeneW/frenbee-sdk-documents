The `FrenbeePhysics component` holds physical definitions for Frenbee. More specifically, it refers to the source data to be applied to an [[Avatar GameObject]].

```csharp
[System.Serializable]
public class FrenbeePhysics : MonoBehaviour {
	public GameObject Avatar; // Edit target
	public List<RigidBody> RigidBodies;
	public List<Fresvii.Frenbee.Joint> Joints;
}
```

The [[FrenbeePhysics component]] is used to define physical definitions for a [[Frenbee Avatar]] and inject a physics-related object into a [[Frenbee Avatar]] manually or automatically when necessary.

> The content of the [[FrenbeePhysics component]] can be edited using the [[Physics Window]].
