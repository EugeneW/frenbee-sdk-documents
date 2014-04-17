## Overview

The `Transitions` of the [[AutomatonState]] currently selected in the [[Automaton States window]] can be edited. The transitions that currently exist are listed. This window lets you edit the content of [[AutomatonTransition]]s.

> An [[AutomatonTransition]] can be added using the [[Automaton States window]].

## How to edit

|GUI|Description|
|---|---|
|Name|Name of the transition|
|`-` button|Removes this transition.|
|Conditions (If all true)|Conditions. This transition is made when all conditions are met.|
|`↑` button|Moves a condition up in the evaluation order.|
|`↓` button|Moves a condition down in the evaluation order.|
|`-` button|Removes a condition.|
|`Time` / `Boolean` / `Float`|Specifies the type of the condition (`AutomatonCondition`). Depending on the type, the items to be edited change (to be described later).|
|`+` button (Add condition)|Adds a new condition.|
|Then go to|Specifies the destination [[AutomatonTransition]] to go to when the conditions are met.|

## How to edit an `AutomatonCondition`

|Type|Description|
|---|---|
|`Time`|A comparison of the normalized time when this state is played and the specified real number (`float`) ([[AutomatonFunction]]) is used as a condition. From the dropdown list, select an [[AutomatonFunction]] as a comparison. For example, 0.0 represents the start time of the animation and 1.0 represents the end time. This is suitable when a transition is made after the animation is played.|
|`Boolean`|An equality comparison (`==`) of the specified Boolean type [[AutomatonParameter]] and the specified Boolean value (`bool`) is used as a condition. As the [[AutomatonParameter]], select one of the Boolean types prepared in the [[Automaton Parameters window]] from the dropdown list. To specify the value, use the checkbox. ☑ (checked) represents `true`, and ☐ (unchecked) represents `false`. This is suitable when using button input or custom true/false fields as a condition.|
|`Float`|A comparison of the specified Float type [[AutomatonParameter]] and the specified real number (`float`) is used as a condition. As the [[AutomatonParameter]], select one of the Boolean types prepared in the [[Automaton Parameters window]] from the dropdown list. This is suitable when using analog stick/analog trigger input or a custom real number as a condition.|

> If multiple conditions are specified, a transition occurs when all of them are met.
> For example, when you set two conditions ("`Time` >= 1.0" and "button input `Boolean` = ☑ (checked)"), whether to make a transition can be evaluated based on whether "the button is pressed at the end of the animation".
