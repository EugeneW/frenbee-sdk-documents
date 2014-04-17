In the Frenbee SDK, several Unity components are available.
> ☞ [About Unity components](http://docs.unity3d.com/Documentation/Manual/UsingComponents40.html)

You can choose necessary components from among these according to purpose.
Some components require other components and are realized through their application.

The following shows the hierarchy of dependencies between required components.
> ☞ [RequireComponent attribute](https://docs.unity3d.com/Documentation/ScriptReference/RequireComponent.html)

(The child component in the hierarchy in the figure shows that its parent component is required. When a component is added to `GameObject`, the missing necessary components will automatically be added by Unity.)

* [[FrenbeeDocument component]]: used to display or animate a 3D model (avatar) from [[Frenbee Document]].
  * [[FrenbeeAvatarAspect component]]: used to perform dynamic model integration of a [[Frenbee Avatar]] (costume change, etc.).
  * [[FrenbeeAutomaton component]]: used to control a [[Frenbee Avatar]] as an Automaton (Animation state machine).
    * [[FrenbeeInputParameterBridge component]]: used to pass input by Input Manager to the Automaton parameter.
* [[FrenbeeModel component]] manages a model in a FrenbeeDocument. Normally managed by the [[Frenbee Document]]. Automatically uses the SkinnedMeshRenderer component and the MeshFilter component of Unity.
* [[FrenbeePhysics component]]: used to add physical motion to a 3D model (avatar) by [[Frenbee Physics]]. Set in the Physics field of a [[Frenbee Document]].
