## Restrictions for conversion

### On supported FBX file formats

* Only the "Embed Media" and "ASCII" format of "FBX 2013.3" is supported.
  * If possible, specify either of this format on the DCC side.
  * An FBX file of any other format needs to be converted in advance using FBX Converter 2013 or later.

### On the model

* The model must be polygons (not curved surfaces).
  * It is strongly recommended to triangulate the model in advance.
  * A normal must be included.
    * Make sure that the normal is not 0 vector. (general caution).
  * One Texture UV set must be included (for the time being).
    * Only the UV format texture is supported.
* On bones
  * Keep the states of reference Avatar model unchanged.
  * Only the Default Names of [[Frenbee Document]]s are mutually converted.
  * As for Bone Index/Weight, a [[Frenbee Document]] may store data of up to four bones per vertex. Select up to four bones having the largest absolute weight values. Others are removed, and the weight total is normalized to 1.
    * Avoid a vertex with zero weight or without a bone (general caution).
    * Restrictions on rendering depend on the rendering engine and its settings. (With Unity, rendering may be performed with the maximum value being 2, depending on the settings.)

### On multiple models

* Conversion involving multiple models is supported in a limited manner.
  * Only the first model that is processed supports bone processing (for the time being).
  * The first model that is processed is used for the bone structure of the animation.
  * Non-bone models ignore coordinate transformation (for the time being).

### On texture

* Diffuse, Ambient, Specular / Specular Power (Shininess), and Emissive are supported.
  * Diffuse is the only texture.
* Alpha/Transparent is not supported.

### On images

* Images can be converted within the limitation of the Unity texture resolution. In the case of an image exceeding the limitation, such as an excessively large image, Unity produces an image of 8 x 8 pixels with a red question mark on a white background.
* Only Embed Media PNG images of the FBX format are supported.

### On animations

* Bone animation conversion depends on the bind pose of the skinned model.
  * When bone animations are mutually converted, they need to include the corresponding skinned models.
* It is necessary to freeze and reduce the animation key frames.
  * A total of six channels are required for translation (x, y, and z) and rotation (x, y, and z).
  * The key time must be exactly the same for all these six channels (the number of keys must match and the keys exist during exactly the same period of time).
  * Interpolation information is ignored completely.

### On model, node, and bone creation and modification

The following parameters are not supported and should not be used. The identity needs to be maintained.

#### Transformation parameters

* In FBX/Maya
  * Rotation offset
  * Rotation pivot
  * Pre-rotation
  * Post-rotation
* In 3ds Max
  * Geometric transform translation
  * Geometric transform rotation
  * Geometric transform translation

#### Scaling parameters

* Scaling offset
* Scaling pivot
* Scaling

[Reference] http://download.autodesk.com/us/fbx/20112/FBX_SDK_HELP/index.html?url=WS1a9193826455f5ff1f92379812724681e696651.htm,topicNumber=d0e7429

