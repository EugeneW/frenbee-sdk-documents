This represents a transition between [[AutomatonState]]s.

## Component elements

|||
|---|---|
|Conditions|Condition for a transition to occur ([[AutomatonCondition]]). Zero or more conditions can be set. Conditions are met if all are `true`. If the number of conditions is 0, it is always regarded as `false`.|
|Name|Name of the transition (not used in the current system)|
|Next|Name of the destination [[AutomatonState]]|