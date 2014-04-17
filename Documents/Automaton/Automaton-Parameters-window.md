## Overview

The Automaton Parameters Window is used to edit the list of the parameters ([[AutomatonParameter]]s) that a [[Frenbee Automaton]] has. The [[AutomatonParameter]]s can be used in the conditions ([[AutomatonCondition]]s) for the transition from one [[AutomatonState]] to another [[AutomatonState]] ([[AutomatonTransition]]).

The values specified here become the initial values used at the start of execution.

## How to edit a parameter

|GUI|Description|
|---|---|
|`-` button|Removes this [[AutomatonParameter]].|
|Name|[[AutomatonParameter]] name. It must be unique in the [[Frenbee Automaton]].|
|Value|Value of a real number (`float`) in the case of a Float type [[AutomatonParameter]].<br>Boolean value (`bool`) in the case of a Boolean type [[AutomatonParameter]]. ☑(checked) represents `true`, and ☐(unchecked) represents `false`.|
|`+` button (Add parameter)|Adds a new [[AutomatonParameter]]. From the context menu ☰ that appears when you click the button, select the type (Float or Boolean) and create a new [[AutomatonParameter]].|


