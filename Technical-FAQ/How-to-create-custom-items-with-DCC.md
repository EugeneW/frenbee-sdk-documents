## How to create custom items

This explains how to create a [[Partial Model]].  Each step has options but the following explains the typical procedure.

1. In DCC where functional components available to Frenbee Avatar can be handled, import a Frenbee Avatar or custom 3D model (via FBX format).
2. Edit the model.
 * In case of hybrid use, custom items and standard items are used together.  Please be careful not to destroy the [[Standard Bones]] status.
3. Save the complete model as a file (for backup).
4. Carefully cut the necessary parts for [[Partial Model]] as Mesh (see below) and save it as a different file (FBX, etc.).
5. Convert the file to [[Frenbee Document]] format.
6. Add the [[Frenbee Document]] to [[Frenbee Paged Assets]] in [[Assets window]].
7. Use models added to [[Frenbee Paged Assets]].

## Note for Cutting out Partial Models

* If you need to cut a part of Mesh of the models, previous normal lines should be maintained even after the cutting out.
 * If the normal lines change because of the cutout, even if [[Model Integration]] is again reapplied to each [[Partial Model]], the joint line of the normal lines becomes discontinuous and the seam becomes visible depending on shading.
 * In this case, check tools / workflow that allow fixing the normal lines and other structures.
* When using a model for [[Model Integration]], it is important to keep the original structure of each Bone from any parentless root Bones with the present ones as well as Bones necessary for deformation of Mesh of the model.  These Bones must be maintained regardless of any residue of the Mesh.