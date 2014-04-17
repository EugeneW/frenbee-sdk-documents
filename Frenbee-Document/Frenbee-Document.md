▶ Frenbee Document

---

A Frenbee Document refers to a document (DOM) that can store the 3D models, animations, and other elements that a [[Frenbee Avatar]] needs, as well as to its file format.

The Frenbee Document is the basic data format used to manage [Frenbee Avatars](Frenbee Avatar) with [[Unity Frenbee Extensions]].

### Related information

* The [[Frenbee Repository]] format is available for managing and editing multiple Frenbee Document files.
* The [[Frenbee Paged Assets]] format consisting of multiple files and folders is available as a modified file format for the Frenbee Document for package bundling.

## How to handle the details of a Frenbee Document

[[Unity Frenbee Extensions]] enable high-level [[Frenbee Avatar]] operations. If necessary, it is possible to program [[Frenbee Document]] read/write and detailed operations through [[Frenbee Core]] APIs.

## Frenbee Document specification

The following table lists the functions, concepts, and terms related to the Frenbee Document. These are useful in creating Developer Items or programming details from the [[Frenbee Core]]. For specific data representations, the type names in XML representations and C# code as well as the relationships between property and field names are shown.

||||
|---|---|---|
|[[Id]]|[[Aspect Item]]|
|[[Outline]]|[[Folder]]|[[Remover]]|
|[[Thumbnail Image]]|
|[[Avatar Creation]]
|[[Avatar Aspect]]|[[Default Aspect]]|[[Avatar Setting]]|
|[[Semantics]]|[[Machine Keywords]]|[[Search Keywords]]|
|[[Document Registry]]|
|[[Model Integration]]|[[Integrated Model]]|[[Partial Model]]|
|[[Bone Integration]]|[[Standard Bones]]|[[Additional Bones]]|

### Types

Specification of the types and formats used in relation to the Frenbee Document

|||
|---|---|
|[[CSV]]|[[DateTime]]

## Frenbee Document file name extensions

* Default: `.fren`

## Overview of the Frenbee Document file format

* The ZIP format is used for containers. For the time being, the ZIP format, not the ZIPX format, is supported.
 * In principle, two files - UTF-8 XML format `index.xml` and binary format `index.bin` - are contained.

## Guidelines for the Frenbee Document

* In principle, use Unicode for character strings. In files, UTF-8 encoding should be used in principle.
* To represent dates and times, use [[DateTime]].
* When an attribute consists of multiple values, use the [[CSV]] format.

