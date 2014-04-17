## Utility Package file distributed on the Frenbee SDK

The following is the procedure for users experiencing the Frenbee SDK for the first time.

1. Install Unity version 4.3 or later on your development machine and create a new Unity project.
2. Currently, the following `unitypackage` files are distributed in the Frenbee SDK. Prepare the latest `FrenbeeSDK***.unitypackage` and `FrenbeeRepository***.unitypackage` files.

> *** indicates the version name.

|File name|Outline|
|---|---|
|`FrenbeeSDK***.unitypackage`|Frenbee SDK. Contains the runtime package for processing Frenbee, Unity editor extensions, etc. [[Unity Frenbee Extensions]], [[Frenbee Core]], etc., are included in this package. |
|`FrenbeeRepository***.unitypackage`| Unity assets compiling [[Partial Model]]s for [[Frenbee Avatar]], [[Aspect Item]]s for [[Integrated Model]], or [[Frenbee Animation]] in the  [[Frenbee Repository]] format. Contains data of 3D models or animation. Import this package into your Unity project together with the Frenbee SDK. Once [[Frenbee Asset Build]] is completed, these assets will become [[Frenbee Paged Assets]]. |

## Importing Unity extensions (Unity Frenbee Extensions).

First, import unitypackage of [[Unity Frenbee Extensions]] to your Unity project.

1. Prepare a project flow with which you would like to use the Frenbee SDK in Unity version 4.3 or later.
 * Create a new project (Main Menu ☰ `File`/`New Project`) or open an existing project.
2. Import `FrenbeeSDK***.unitypackage`.
 * Main Menu ☰ `Assets`/`Import Package`/`Custom Package...`
 * Select `FrenbeeSDK***.unitypackage` in the dialog box. (The *** part differs for each version.)
 * When an error occurs, it may be resolved by updating Unity to the latest version.
3. `Frenbee` has been added to the Main Menu ☰. The Unity editor extensions has also become available.

> Install the Frenbee SDK for each project for which the SDK is used.

## Installing Frenbee Repository

Next, install the standard 3D models or animation assets for [[Frenbee Avatar]]. These assets are contained in `FrenbeeRepository***.unitypackage` in the [[Frenbee Repository]] format.

1. Use the same project used for the previous process.
2. Import `FrenbeeRepository***.unitypackage`.
 * Choose from the Main Menu ☰ `Assets`/`Import Package`/`Custom Package...`
 * Select `FrenbeeRepository***.unitypackage` on the dialog box. (The *** part differs for each version.)
 * When an error occurs, it may be resolved by updating Unity to the latest version.
3. Wait until the package has been imported. When [[Frenbee Asset Build]] completes import processing, [[Frenbee Paged Assets]] is generated.
4. Standard [[Frenbee Avatar]] assets are now available for each Frenbee SDK function.

> Install the Frenbee SDK for each project for which the SDK is used.

View a sample scene to check whether a proper environment is provided.

1. See ☞ [[Demos]].
