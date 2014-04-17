`AutomatonParameter` represents the parameter used for [[Frenbee Automaton]].
It can be edited using the [[Automaton Parameters Window]].

##Scripting

|Property/field|Description|
|---|---|
|`Type`|AutomatonParameterType enumeration indicating the parameter type. It is either `Float` or `Boolean`.|
|`Name`|[[AutomatonParameter]] name. This must be unique in [[Frenbee Automaton]].|
|`BooleanValue`|Current Boolean value (`bool`) (`true` or `false`) used for the Boolean type [[AutomatonParameter]]|
|`FloatValue`|Current real number (`float`) used for the Float type [[AutomatonParameter]]|

### `AutomatonParameter` types

`AutomatonParameter` is shared among the multiple usages mentioned below. The usage is identified by the value of `AutomatonParameter.Type`. While multiple values are held, the valid value is the one that corresponds to the usage indicated by `AutomatonParameter.Type`.

* Float type `AutomatonParameter`
* Boolean type `AutomatonParameter`

> In the [[Automaton Parameters Window]], the usage is determined when `AutomatonParameter` is created.

### Setting the value from the script

The following methods allow the value to be set from the script easily.

```csharp
Automaton.Set(string parameterName, bool value);
```
```csharp
Automaton.Set(string parameterName, float value);
```

