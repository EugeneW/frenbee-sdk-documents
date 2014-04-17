The `FrenbeeDocument component` enables rendering of a 3D [[Frenbee Avatar]].
In principle, one `FrenbeeDocument component` displays one [[Frenbee Document]].

The following are the major usages of the FrenbeeDocument component:

## When loading a single Frenbee Document

1. The `FrenbeeDocument component` loads each model contained in the specified [[Frenbee Document]] as a `GameObject` having a [[FrenbeeModel component]].

## When building an integrated model from multiple Frenbee Documents indicated by Avatar Aspect

1. the `FrenbeeDocument component` loads each [[Frenbee Document]] indicated by the specified Avatar Aspects from [[Frenbee Paged Assets]],
2. and builds a [[Frenbee Document]] containing a single [[Integrated Model]].
3. The component loads this [[Frenbee Document]] in the manner previously described.
