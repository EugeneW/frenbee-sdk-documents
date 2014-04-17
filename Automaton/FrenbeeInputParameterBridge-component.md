> The use of the `FrenbeeInputParameterBridge component` is optional.

## Overview

The `FrenbeeInputParameterBridge component` copies specific input values of the Input Manager of Unity to specific [[AutomatonParameter]] on a per-frame basis.
You can use this component when you want to use the input from the Input Manager as parameter values. In applications where `FrenbeeInputParameterBridge` is applicable, it is not necessary to prepare a unique script.

## Tip

Define unique parameters, and write a script in which the parameter values change with the game state. This enables more advanced automaton control.

## How to edit

Use the `Inspector` window of the `FrenbeeInputParameterBridge component`. The window contains the Axes and Buttons lists as described below.
Expand, reduce, or edit these lists as appropriate for the Input Manager and Automaton Parameters.

> Since the Input Manager of Unity 4.x has no explicit API to obtain the names of the existing Axes, they need to be managed manually.
When you make a change to the Input Manager, uncheck the Enabled box for each nonexistent Axis name or delete it.

### Axes list

The list is set to read the Axes of the Input Manager using `Input.GetAxesRaw` and bridge them to a Float parameter.

|||
|---|---|
|Enabled|Check this box when enabling this bridge.|
|Source|Name of the source Axes of the Input Manager|
|Target|Name of the destination Automaton Parameter|

### Buttons list

The list is set to read the Axes of the Input Manager using `Input.GetButton` and bridge them to a Boolean parameter.

|||
|---|---|
|Enabled|Check this box when enabling this bridge.|
|Source|Name of the source Axes of the Input Manager|
|Target|Name of the destination Automaton Parameter|

### Context menu ☰ `Edit Input Manager`

Open the Input Manager.
> Same as main menu ☰ `Edit`/`Project Settings`/`Input`
