# MysteryPancake's Rule Book
## GitHub
* Editing code directly on this site must not occur (too often).
* Repository names must have capital letters at the start of each word.
* Repository names must use `-` to separate words.
* Repository names must be as short as possible.
* Repository descriptions must not have a full stop.
* Repository descriptions must be as short as possible.
* Repositories intended for personal use must have an `MIT License` with `MysteryPancake` as the legal name.
* Repositories intended for external use must have no license.
* Images in `README` files must be hosted on the repository, not an external site.
* Small unused scripts must be added to the [Fun repository](https://github.com/MysteryPancake/Fun).

## Lua
* All variables must be initialized as `local`.
* Tab indentation must be used, not spaces.
* Spacing must remain consistent and look nice.
* Tables must be sequential where possible.
* Variables must never be initialized as `local var = var` unless in a module.
* Spaces must be on both sides of `..`.
* Strings must have `"`, not `'` unless `[[` and `]]` are required.
* Expressions such as `x = x * 0.75` must be used, not `x = x - x / 4`.
* `(` and `)` must not be used unless required.
* Sequential tables must be iterated with `ipairs`, not `pairs`.
* Unused function return values must be set as `_`.
* Unused keys or values in a `for` loop must be set as `_`.
* `;` semicolons must never be used.
* Variable names must be in camelCase as well as functions.
* Variables must be named `str`, not `txt`.
* Variables must not be the name of an existing object.
* `math.random( 1, n )` must be `math.random( n )`.
* To choose a random boolean `math.random() > 0.5` must be used.
* `While` and `until` loops must be avoided in favour of `for` loops.
* `math.randomseed` must never be used.

## Garry's Mod
* Repositories intended for external use must be named with the style of `GMod-Insert-Name-Here`.
* Repositories must have the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod` and `gmod-lua`.
* Repositories must have a link to the addon.
* STOOL repositories must have the tag `garrysmod-tool`.
* Repository descriptions must have the style of `Insert Name Here for Garry's Mod`.
* `AddCSLuaFile` must never be used for `lua/autorun` files.
* Hooks must use functions not set to a variable.
* `Panel` must be used, not `DPanel`.
* `and`, `or` and `not` must be used, not `&&`, `||` and `!`.
* Functions with default arguments must not be called with the argument unless overriding.
* Repositories must have an addon icon image and the associated Photoshop file.
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
* Projects must have a full icon set.
* Errors must be handled properly.

## Swift
* Ranges in `for` loops must not have spacing on either side.
* Double spaced indentation must be used, not tabs.
* Variables must be declared as `private` unless required by the compiler.
* No variables must be above the level of `internal`.
* Where possible `===` and `!==` must be used, not `==` or `!=`.
* No variables must be type declared except for numbers.
* Division must never be used as it is slower than multiplication.
* Expressions such as `x *= 0.75` must be used, not `x = x - x / 4`.
* `(` and `)` must not be used unless required.
* Variables must use `get`, `set` and `didSet` where possible.
* `?` weak and `!` implicitly unwrapped variables must be avoided.
* Arrays are preferred over sets.
* Classes must be marked as `final` unless intended to be overridden.
* Overridable classes must have as many variables as possible marked `final`.
* Unused variables must be set as `_`.
* Structs must be used over classes where possible.
* `arc4random` and `arc4random_uniform` must be used for random number generation.
* `DispatchQueue` must be avoided.
* `SKShapeNode` must never be used as it leaks memory.
* Wrappers must be avoided in favour of bases.
* Extensions must be used to reduce namespace clutter.
* Variables must be marked as `let` unless the compiler requires `var`.
* Arrays must be initialized with the style of `x: [Int] = []`, not `x = [Int]()`.
* Dictionaries must be initialized with the style of `x: [Int: Int] = [:]`, not `x = [Int: Int]()`.
* Arrays with repeated values must be initialized with the style of `x: [Int] = Array(repeating: 1, count: 2)`.
