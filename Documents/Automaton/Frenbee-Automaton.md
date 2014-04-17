A Frenbee Automaton is a function that controls the state transition of a [[Frenbee Animation]] for a [[Frenbee Avatar]] as an automaton (animation state machine). The [[FrenbeeAutomaton component]] represents and executes the automaton.

A Frenbee Automaton consists of the elements listed below.

|Type|Name|Outline|
|---|---|---|
|[[AutomatonState]]| State| State in which a certain animation is played |
|[[AutomatonTransition]]| Transition| Represents a transition from one state to another. It consists of the destination state, conditions, etc. The transition occurs when the conditions are met. |
|[[AutomatonCondition]]| Condition| Condition for a transition to occur |
|[[AutomatonParameter]]| Parameter| Input parameter used as a transition condition. A parameter unique to a specific game can be defined. Set user-input or a change in the game state as a parameter. Or, use the [[FrenbeeInputParameterBridge component]]. |

The content of a Frenbee Automaton can be edited using the [[Automaton States Window]], [[Automaton Transitions Window]], or [[Automaton Parameters Window]].

## How a Frenbee Automaton works

A Frenbee Automaton can be controlled dynamically using either or both of the following methods.

* Link user-input using the [[FrenbeeInputParameterBridge component]].
* Let the value of the [[AutomatonParameter]] change dynamically when executed from the script.

These enable the [[Frenbee Automaton]] to be controlled based on the relationships described below.

1. The [[AutomatonCondition]] value is changed as mentioned above.
2. The evaluated result of the [[AutomatonCondition]] in the [[AutomatonTransition]] changes.
3. When the evaluated result is `true`, the corresponding state transition occurs.
4. As a result, the [[AutomatonState]] of the [[Frenbee Automaton]] changes.

## See also

* ☞ [[FrenbeeAutomaton component]]
* ☞ [[Automaton States Window]]
* ☞ [[Automaton Transitions Window]]
* ☞ [[Automaton Parameters Window]]
* ☞ [[FrenbeeInputParameterBridge component]]