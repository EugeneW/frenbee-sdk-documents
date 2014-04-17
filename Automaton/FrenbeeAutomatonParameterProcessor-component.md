The FrenbeeAutomatonParameterProcessor provides dynamic [[AutomatonParameter]] values exclusively intended for a specific purpose.
In principle, the output [[AutomatonParameter]] is updated based on the result of processing the specific input [[AutomatonParameter]] on a per-frame basis.

The currently available function is as follows.

|Type|Output [[AutomatonParameter]]|Description|
|---|---|---|
|`float`|Movement|Represents the user-input amount of avatar movement. It is the result synthesized from the user-input horizontal movement `Horizontal` (``float``) and the user-input vertical movement `Vertical` (``float``). The value of Movement is used as an example of the [[FrenbeeAutomaton component]] in the Action Runner Demo. See ☞ [[Demos]].|

> For this component to function, the input and output [[AutomatonParameter]]s of the appropriate type mentioned above need to be prepared in [[AutomatonParameter]] of the [[FrenbeeAutomaton component]].
