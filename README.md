# mir-random
Dlang Random Number Generators

#### Comparison with Phobos
 - Does not depend on DRuntime (Better C concept)

##### Generators
 - `opCall` API instead of range interface is used (similar to C++)
 - No default and copy constructors are allowed for generators.
 - 64-bit Mt19937 initialization is fixed
 - 64-bit Mt19937 is default for 64-bit targets
 - `unpredictableSeed` has not state, returns `ulong`
 - `@URNG` UDA is used for for RNGs instead of a enum flag.
 - `min` and `max` proporties was removed. Generators must always generate uniformly all set of bits.
 - Any unsigned generators are allowed.
 - `LinearCongruentialEngine` was removed.
 - [WIP] additional Xorshift generators

##### Integer uniform generators
[WIP]

##### Real uniform generators
[WIP]

##### Nonuniform generators
[WIP]
