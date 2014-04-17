To create a [[Folder]] item of the [[Frenbee Document]], do the following. Note - In this sample procedure, it is assumed that a [[Folder]] item of [[Aspect Item]] has been created.

> In this procedure, a [[Folder]] item of the [[Frenbee Document]] and a folder as a file system (as assets in Unity) are used.  Please carefully read the explanation.

1. Display the [[Frenbee Repository]] folder in the `Project` window.
2. Choose the `Aspect` folder and move it into the folder (in case of creating a [[Folder]] item of [[Aspect Item]]).
3. Use sub-folders (`folders`, etc) to organize items if you want further refinement for the items.  For example, for making prototypes, this approach makes your work easy, such as deleting items later.
3. Make a new [[Frenbee Document]] using [[How to create a new item with Id]].  If you use an existing [[Frenbee Document]], proceed to the next step.
4. Select a [[Frenbee Document]] to be edited and choose from the context menu ☰ `Frenbee`/`Repository`/`Edit Outline` (by right clicking, etc.) to open the [[Outline window]] window. 
5. Edit [[Outline]] in the [[Outline window]] window as described later.
6. Save the edited [[Frenbee Document]] by clicking the `Save` button.
7. The saved [[Frenbee Document]] is automatically published in [[Frenbee Paged Assets]] by [[Frenbee Asset Build]].
8. Click the`Reload` button to check the action of the edited item in the [[Aspect window]]. Repeat the step 5 through 8 until the desired result is obtained.

## Edit Outline as Folder

* Enter meaningful name in the `Name` box. This will be the display name.
* Select [[Gender]] if you want (i.e., for a Male or Female dedicated folder).
* Set [[Machine Keywords]] in [[CSV text field]] format.  This [[Folder]] contains the keywords to be searched from the other [[Folder]] (such as parents, etc.). In addition, one of three, `both`, `male`, `female`. must be included as per the [[Gender]] settings.
* Select `This is a folder` checkbox ☑ (checked). This setting is important for it to work as [[Folder]].
* Set `+ Machine Keywords` in [[CSV text field]] format.  This is required for virtual child items.
* Set `- Machine Keywords` in [[CSV text field]] format.  This is required to exclude for virtual child items.  Generally, `obsolete` should be included.
* If appropriate, you can set [[Thumbnail Image]] by clicking the `Import...` button to import a PNG file.

> Settings of Machine Keywords, `+ Machine Keywords` and `- Machine Keywords` of each [[Folder]] item determine the relationship among [[Folder]] items.  Refer to the existing [[Folder]] items.
The above is only a summary and some items are not explained here. Please see ☞ the [[Outline window]] for details.
