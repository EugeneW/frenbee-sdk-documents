The Automaton States window lets you graphically edit the state transition diagram of a [[FrenbeeAutomaton component]]. In the upper part of the window, you can perform the operations below.

|GUI|Description|
|---|---|
|Automaton|Specify the `GameObject` that has the [[FrenbeeAutomaton component]] to be edited here.|
|Playing state|Indicates the playing [[AutomatonState]].|
|Selected state|Indicates the [[AutomatonState]] currently selected in the edit window.|
|Margin|The margins of the transition diagram in the edit window can be adjusted.|
|☑Quantization|When this box is checked (☑), the layout is automatically quantized during the editing of the transition diagram.|
|Unit|The unit of layout quantization can be adjusted.|

## How to edit the state transition diagram

The lower part of the window shows the state transition diagram. A rectangle represents an [[AutomatonState]], and a curve represents an [[AutomatonTransition]].
You can select the rectangle of an [[AutomatonState]] by left-clicking it.

### Context menu ☰ of an AutomatonState rectangle

If you right-click on an [[AutomatonState]] rectangle, you can use the following context menu functions.

|Context menu ☰|Description|
|---|---|
|`Set as default`|Sets an [[AutomatonState]] as the default.|
|`Remove`|Removes an [[AutomatonState]].|
|`Make a transition from selected state to this` (only for an [[AutomatonState]] not currently selected)|Adds an [[AutomatonTransition]] (curve) from the currently selected [[AutomatonState]] to this [[AutomatonState]].|

### Frame context menu ☰

If you right-click anywhere other than an [[AutomatonState]] rectangle, you can use the following context menu functions.

|Context menu ☰|Description|
|---|---|
|`+`|Adds a new [[AutomatonState]].|
|`Add transited state`|Adds a new [[AutomatonState]]. This also adds a new [[AutomatonTransition]] (curve) from the currently selected [[AutomatonState]] to the new [[AutomatonState]].|