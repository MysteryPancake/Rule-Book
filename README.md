# My Rule Book
## GitHub
* Editing code directly on this site must not occur (too often).
* Repository titles must have capital letters at the start of each word.
* Repository titles must have `-` instead of spaces.
* Repositories intended for personal use must have an `MIT License` with `MysteryPancake` as the legal name. Otherwise, no license must be included.
* Repository descriptions must be as short as possible.
* Repository descriptions must not include a full stop.
* Small unused scripts must be added to the [Fun repository](https://github.com/MysteryPancake/Fun).
* Images in `README` files must be hosted on the repository, not an external site.

## Lua
* Tables must be sequential where possible.
* Variables must be declared as `local`.
* Tabs must be used, not spaces.
* No variables must be declared as `local var = var`, unless in a module.
* Spacing must remain consistent and look nice.
* Spaces must be on both sides of `..`.
* Strings must have `"`, not `'`, unless `[[` and `]]` are required.
* Expressions such as `x = x * 0.75` must be used instead of `x = x - x / 4`.
* `(` and `)` must not be used unless required.
* Sequential tables must be iterated with `ipairs`, not `pairs`.
* Unused function return values must be set as `_`.
* Unused keys or values in a `for` loop must be set as `_`.
* `;` semicolons must never be used.
* Variable names must be in camelCase as well as functions.
* Variables must be named `str` instead of `txt`.
* Variables must not be the name of an existing object.
* `math.random( 1, n )` must be `math.random( n )`.
* To choose a random boolean, `math.random() > 0.5` must be used.
* `While` and `until` loops must be avoided in favour of `for` loops.
* `math.randomseed` must not be used.

## Garry's Mod
* Repositories intended for external use must be named `GMod-Insert-Name-Here`.
* Repositories must have the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod`, and `gmod-lua`.
* Repositories must have a link to the addon next to the description.
* If the repository is for a STOOL, then the tag `garrysmod-tool` must also be included.
* Repository descriptions must be `Insert Name Here for Garry's Mod`.
* `AddCSLuaFile` must never be used for `lua/autorun` files.
* Hooks must use functions not set to a variable.
* Repositories must include an addon icon image and the associated Photoshop file.
* Repository `README` files must be structured as the following:

```
# Garry's Mod NAME
All the code for my NAME addon can be found here, and the actual addon is available [here](ADDON LINK).
![Icon](ICON PATH?raw=true)
```

## XCode
* Every warning must be enabled.
* The iOS requirement must be kept as low as possible.
* Warnings must be treated as errors.
* Projects must include a full icon set.
* Errors must be handled properly.

## Swift
* Variables must be declared as `private`, unless required by the compiler.
* No variables must be above the level of `internal`.
* `===` and `!==` must be used instead of `==` and `!=` where possible.
* No variables must be type declared, except for numbers.
* Division must never be used, as it is slower than multiplication.
* Expressions such as `x *= 0.75` must be used instead of `x = x - x / 4`.
* `(` and `)` must not be used unless required.
* Variables must use `get`, `set`, and `didSet` where possible.
* `?` weak and `!` implicitly unwrapped variables must be avoided.
* Arrays are preferred over sets.
* Classes must be marked as `final` unless intended to be overwritten.
* Overwritable classes must have as many variables as possible marked `final`.
* Unused variables must be set as `_`.
* Structs must be used over classes where possible.
* `arc4random` and `arc4random_uniform` must be used for random number generation.
* `DispatchQueue` must be avoided.
* `SKShapeNode` must never be used, as it leaks memory.
* `UIBezierPath` must be avoided in favour of `CGPath`, as it is a wrapper.
* To remove an element from an array, `array = array.filter { $0 !== element }` must be used.
* Extensions must be used to reduce namespace clutter.
* Variables must be marked as `let` unless the compiler requires `var`.
* Collections must be initialized with the style of `x: [Int] = []`, rather than `x = [Int]()`.
