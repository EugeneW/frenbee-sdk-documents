▶ [[Frenbee Document]]

---

Avatar Setting is information mainly used to change the appearance of an avatar by processing the specific information that comprises the [[Integrated Model]] of the [[Frenbee Avatar]]. Specifically, it is used to replace a material color or texture name or a morph value. Generally, a list of 0 or more Avatar Settings is compiled in a [[Frenbee Document]] and used as an item.

> In [[Frenbee Core]], the structure can be represented in C# code as shown below. Note that, in this code, the `null` check and element count check are omitted.
```csharp
var setting = Document.Avatars[0].Aspects[0].Settings[0];
```

## Frenbee Document / XML

The Avatar Setting is represented as an `AvatarSetting` element in the XML code of its [[Frenbee Document]]. The basic structure of this element is as follows.

|Attribute|Description|
|---|---|
|`Method`|Name of the method of processing. The available methods are described later.|
|`Target`|Condition for the target name (mainly the match of the leading portion of a string). The target element is determined by the method.|
|`Source`|Original value to produce the result of processing. The type and XML notation of this value is determined by the method.|

## Available methods

|Method|Target|Source|Description|
|---|---|---|----|
|`SetMaterialAmbientColor`|Leading portion of the target mesh name (multiple matches acceptable)|`Vector3` representation of RGB colors|The source color is set to the ambient color of the material that the target mesh has.|
|`SetMaterialDiffuseColor`|Leading portion of the target mesh name (multiple matches acceptable)|`Vector3` representation of RGB colors|The source color is set to the diffuse color of the material that the target mesh has.|
|`SetMaterialSpecularColor`|Leading portion of the target mesh name (multiple matches acceptable)|`Vector3` representation of RGB colors|The source color is set to the specular color of the material that the target mesh has.|
|`SetMaterialTexture`|Leading portion of the target mesh name (multiple matches acceptable)|Leading portion of the image name|The image that matches the source in the source-side [[Frenbee Document]] is set for the texture of the material that the target mesh has. If no image is found, no texture is set.|
|`SetBackgroundTexture`|This method does not have any particularly effective use in the current Frenbee SDK. Leading portion of the target camera name (multiple matches acceptable)|Leading portion of the image name|The image that matches the source in the source-side [[Frenbee Document]] is set for the background texture of the target camera. If no image is found, no texture is set.|
|`ReferenceMaterial`|Leading portion of the target mesh name (multiple matches acceptable)|Leading portion of the mesh name|The material of the mesh specified by the source in the target [[Frenbee Document]] is searched for as the reference source. If no reference source is found, the method has no effect. If the reference source is found, the source material is set as the reference for the material of the target mesh. Note that the reference source is not the source [[Frenbee Document]].|
|`SetMorphAmount`|Leading portion of the target morph name (multiple matches acceptable)|Leading portion of the morph name|The value of the source is set in the weight (morph value) of the target morph.|

> * In the above table, "leading portion" indicates that the match condition is "the leading portion of a string". Since elements with similar names are handled collectively, the match condition can be specified using only the leading portion of a name.
> * In the above table, "multiple matches acceptable" indicates that, if more than one element meets the condition, the processing applies to all of them.

> In the C# code of [[Frenbee Core]], the following methods are related:
> * Document.IntegrateAvatarSettings
> * Document.ApplyAvatarSettings
> * AvatarSetting.Apply
