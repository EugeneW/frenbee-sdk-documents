In the Frenbee system, an asset consisting of more than one [[Frenbee Document]] is handled in the following formats in two stages.
When compared to a software build, [[Frenbee Repository]] is the source code (input file), and [[Frenbee Paged Assets]] is a software artifact (output file).

The former is the format for performing management and editing, since the individual [[Frenbee Document]] is a single file and easy to manipulate. The latter is a processed format that is suitable for runtime environments.

## Frenbee Asset pipeline

|Stage|Format|Outline|Example of target functions|
|---:|:---:|---|---|
|1|[[Frenbee Repository]]|Format used for creation/editing/management of [[Frenbee Document]]|[[Outline window]]|
|2|↓| Processing by [[Frenbee Asset Build]]|
|3|[[Frenbee Paged Assets]]|Format of [[Frenbee Document]] for runtime/package.|[[Assets window]] / [[Aspect window]]|
