## Overview

An `AutomatonState` represents a state of a [[Frenbee Automaton]]. Basically, an `AutomatonState` is a state in which a specific animation is referenced and played. It has [[AutomatonTransition]]s to a given number of other `AutomatonState`s and indicates that it can transition to another `AutomatonState` when a certain condition is met.

## AutomatonState component elements in the diagram GUI

|GUI|Description|
|---|---|
|D|When this `AutomatonState` is the default state, "D" is shown at the upper left of the rectangle.|
|Name|Name. It is name-referenced as the transition destination. The state name must be unique in the automaton.|
|Transitions|Set of transitions ([[AutomatonTransition]]s). It is represented by a curve from the bottom of the rectangle of this `AutomatonState` to the top of the rectangle of the destination AutomatonState.|
|Animation|Reference to the animation to be played in this `AutomatonState`|

## AutomatonState fields/properties

|Field/property|Description|
|---|---|
|`IsDefault`|`true` when this `AutomatonState` is the default state. The automaton starts in the default state. If no default state exists, the automaton starts in the `null` state.|
|`Rect`|Coordinates of the rectangle of the `AutomatonState` when the diagram is edited|
|`AnimationLink`|String representation of [[Id]] of the animation to be referenced|
|`Animation`|Animation referenced based on the AnimationLink. It is `null` if the AnimationLink is not a valid reference or the animation is not loaded.|
|`RepeatTransformation`|Coordinate transformation synthesized to `Transform` of `GameObject` of [[FrenbeeAutomaton component]] every time the animation reaches the last frame (a loop occurs). It represents a local relative parallel movement (translation) or rotation. Accumulated movements and direction changes of the avatar are explicitly specified. This enables a movement of the [[Frenbee Avatar]], such as continuous walking or rotation, by specifying an explicit value.|