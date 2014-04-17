This is the `F.Physics` window dedicated to editing the content of a [[FrenbeePhysics component]] in a scene. The window is used to edit the [[Frenbee Physics]] definitions.

To be more exact, the Physics window is intended for one `GameObject` in a scene that has a [[FrenbeePhysics component]].
(Make sure that there is only one [[FrenbeePhysics component]] in a scene.)

## Opening the Physics Window

Choose from the Main Menu ☰ `Frenbee`/`Physics Window`.

The [[Frenbee Physics]] edit window is opened.

> The window can also be opened using the `Open Frenbee Physics Window` button of the inspector of the [[FrenbeePhysics component]].
> (Note that, if there are multiple [[FrenbeePhysics component]]s in a scene, the content of another unintended [[FrenbeePhysics component]] may be displayed.)

## If there is no [[FrenbeePhysics component]] in a scene

If there is no [[FrenbeePhysics component]] in a scene, the Physics window displays an error, instead of its standard editing GUI.
* FrenbeePhysics component not found in the scene.

To start editing, first add the "Physics Design" prefab provided by the Frenbee SDK to the scene from the `Project` window.

If necessary, you can create a new "Physics Design" prefab by clicking the `Create a new GameObject with FrenbeePhysics component` button displayed in `F.Physics` of the Physics window.
This creates a new `GameObject` with a [[FrenbeePhysics component]] by the name `Physics Design`.

## `F.Physics` tab

This tab contains the functions to specify an [[Avatar GameObject]] to which to apply (inject) physical settings and manage the [[Avatar GameObject]] physical settings.

|GUI|Description|
|---|---|
|Avatar GameObject| Sets the [[Avatar GameObject]] in the scene to which to write physical settings. (This allows you to include multiple avatars in a scene and set them individually while switching from one to another, enabling a physical test to be run without rewriting the physical settings other than those of Frenbee in the scene.)|
|`Apply to the Avatar` button| Applies physical settings to the [[Avatar GameObject]] (by writing new physical information after deleting the old physical information of the avatar). In this process, the physical elements are used only when they are enabled. (Elements that have failed to be name-referenced are also ignored. The information is output to the log.) Also, the [[Avatar GameObject]] to which physical settings have been applied is automatically selected. This makes the applied physical settings visible for easy identification in the scene window (e.g., the position of the Collider).|
|`Remove all runtime physical objects in the Avatar` button| Removes the physics-related information of the [[Avatar GameObject]] (information irrelevant to Frenbee Physics may be included).|

## `F.Rigid Bodies` tab

This tab is used to edit the list of Frenbee Rigid Bodies. Here, you can edit the content of the [[Rigid Body]] selected in the list.

## `F.Joints` tab

This tab is used to edit the list of Frenbee Joints. Here, you can edit the content of the [[Joint]] selected in the list.

## How to edit the list in the Physics Window

|GUI|Description|
|---|---|
|Slider| Lets you select a list item by moving the list slider.|
|List checkbox| Displays or hides the name list.|
|`List item name` button| Lets you select a list item by clicking the button. (You may use either the slider or this button.)|
|`+` button| Adds a list item.|
|`-` button| Removes a selected list item.|