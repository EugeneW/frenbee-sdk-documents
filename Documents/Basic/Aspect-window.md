The Aspect Window is the `F.Aspect` window for editing the [[FrenbeeAvatarAspect component]]. It allows you to change the avatar appearance in Edit mode or Play mode.

## Outline

* Allows you to perform [[Avatar Creation]] (appearance editing) of an avatar for which dynamic appearance can be modified dynamically in-game ([[FrenbeeAvatarAspect component]]).
* The [[Integrated Model]] of the edited avatar can be saved as a [[Frenbee Document]] so that it can be used as a prebuilt avatar (with a fixed appearance) by clicking the `Save as` button.
* Allows you to change the [[Gender]] and reset the avatar to [[Default Aspect]].
* Allows you to change the current [[Avatar Aspect]] to a compatible [[Aspect Item]].
* Supports [[Folder]], which allows you to edit avatars by moving folders or to check folder behavior. Also equipped with a folder browsing history function.
* Supports [[Remover]], enabling you to check [[Aspect Item]] removal behavior from [[Avatar Aspect]].
* Enables search of [[Aspect Item]]s compatible with the current [[Avatar Aspect]] using an instant [[Folder]].

## Opening Aspect Window

Opens from Main Menu ☰ `Frenbee`/`Aspect Window`.

## Operations

### When editing a general Male or Female avatar

If Current Gender is set to `None` or `Both` or there are no Current Avatar Aspect items, the avatar is not in a normal display status. In this case, reset the avatar using the `Reset to male's default` or `Reset to female's default` button before starting editing the avatar.

|GUI|Description|
|---|---|
|Aspect GameObject| Set a `GameObject` containing the [[FrenbeeAvatarAspect component]] that is edited by the Aspect Window. You can also select a `GameObject` containing the [[FrenbeeAvatarAspect component]] in the `Hierarchy` window. |
|`Reload` button| Loads the latest [[Document Registry]] of the Aspect asset folder. Normally, updates are automatically performed when [[Frenbee Paged Assets]] is modified. Use this button when updates are not automatically performed. |
|`Semantics` toggle| Displays the [[Semantics]] list for confirmation when it is ☑ (checked). This list displays all the [[Semantics]] of each [[Aspect Item]] the current avatar consists of. This list is sorted. |
|Gender|[[Gender]] of the current avatar. |
|`Reset to male's default` button|Set [[Gender]] to Male to reset the avatar to the default appearance. |
|`Reset to female's default` button|Set [[Gender]] to Female to reset the avatar to the default appearance. |
|`Save as` button (only when the avatar can be saved)|Saves the current [[Integrated Model]] as a [[Frenbee Document]] file. In the [[Frenbee Document]], the [[Integrated Model]] corresponding to the current [[Avatar Aspect]]  and the current [[Avatar Aspect]] (AvatarAspect elements) is also saved. |
|Current Avatar Aspect|The current avatar appearance. The following list shows the current [[Aspect Item]] configuration. When the configuration is edited, it is reflected in the 3D avatar on the Game or Scene window. List items can be added from all compatible items. |
|`-` button| Explicitly removes the current [[Aspect Item]]. |
|Current folder|The current (virtual) [[Folder]]. |
|`Back` button|When there is a previous [[Folder]] in the folder browsing history, returns to the [[Folder]]. |
|`Show aspect base folder` button|Moves to the Aspect base folder for developers in the aspect asset and resets the folder browsing history. When no appropriate [[Folder]] items are found in the aspect asset, a warning message will be displayed. |
|`Show aspect home folder` button| Moves to the default Aspect home folder for in-game purpose in the aspect asset and resets the folder browsing history. When no appropriate [[Folder]] items are found in the aspect asset, a warning message will be displayed. |
|`Show all aspect items` button|Moves to the All aspect items [[Folder]] and resets the folder browsing history. This folder displays all items compatible with the current Avatar Aspect excluding `obsolete` items. This folder always functions independent of the aspect asset. This button is effective when no appropriate [[Folder]] items are found in the aspect asset.. |
|Name|[[Folder]] name|
|Id|[[Folder]] [[Id]]|
|+ Machine Keywords|The "Including Machine Keywords" condition of the [[Folder]]|
|- Machine Keywords|The "Excluding Machine Keywords" condition of the [[Folder]]|
|`Search by instant folder` toggle|Search function (explained in detail in the following). |
|Compatible items|Displays items compatible with the current avatar configuration (the configurations are interchangeable) in the [[Frenbee Paged Assets]] (explained in detail in the following). Compatibility here means conforming to the conditions of the Current folder or [[Gender]]. |

## Search by instant folder

"Search by instant folder" is a check function that searches items using [[Machine Keywords]] as the conditions using an instant [[Folder]]. 
* When its status is ☑ (checked), the instant folder is set as the Current folder.
* When its status is ☐ (unchecked), the instant folder returns to the previous folder.

When +MKs and -MKs are input in the [[CSV text field]] format or changed by each button, search will start immediately. The search result items are displayed in Compatible items. These items can be operated in the usual manner.

> When there are too many items, some delay will occur in [[Thumbnail Image]] loading.

|GUI|Description|
|---|---|
|Valid Machine Keywords on Paged Assets|Displays a list of [[Machine Keywords]] in the current [[Frenbee Paged Assets]]. The following operations can be performed using the button on the left of each [[Machine Keywords]] item. |
|`-` button|Add the keyword to the "Excluding Machine Keywords" condition. Remove the keyword from the "Including Machine Keywords" condition. |
|` ` button|Remove the keyword from the Machine Keywords conditions (the keyword will not be included in the "Including Machine Keywords" and "Excluding Machine Keywords" conditions). |
|`-` button|Add the keyword to the "Including Machine Keywords" condition. Remove the keyword from the "Excluding Machine Keywords" condition. |
|+MKs|Including Machine Keywords of the instant `Folder`. Keywords can be entered directly in the [[CSV text field]] format or changed using the buttons under Valid Machine Keywords on Paged Assets. |
|-MKs|Including Machine Keywords of the instant `Folder`. Keywords can be entered directly in the [[CSV text field]] format or changed using the buttons under Valid Machine Keywords on Paged Assets. |

## Types of items displayed under Compatible items

### [[Aspect Item]]

"Aspect" is displayed on the left. When the button of the item name is clicked, the item will be applied (added or replaced) to the Current Avatar Aspect list.
By clicking the `Preview` button, you can check how the a single [[Aspect Item]] is displayed. In this case, no change will be made to the Current avatar aspect list.

### [[Folder]]

"Folder" is displayed on the left.
By clicking the button of the item name, the item will move to [[Folder]]. The Current folder will be updated and added to the folder browsing history.

### [[Remover]]

"Remover" is displayed on the left.
When the button of the item name is clicked, the [[Aspect Item]] group with the applicable [[Semantics]] will be removed from the Current Avatar Aspect list.
