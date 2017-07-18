# MysteryPancake's Rule Book
## GitHub
* Editing code on the site must be avoided, except for this guide.
* All repository titles must have capital letters at the start of each word.
* All repository titles must have `-` instead of spaces.
* All repositories intended for personal use must have an `MIT License` with `MysteryPancake` as the legal name. Otherwise, no license must be included.
* All repository descriptions must be as short as possible.
* All repository descriptions must not include a full stop.
* Small pieces of code must be added to the Fun repository.
* Images must be hosted on the repository, not an external site.

## Rule Book
* Rules must be kept as short as possible.
* Australian spelling must be used.
* `Instead of` must be used instead of `over`.
* `Where` must be used instead of `when`.
* All titles must have capital letters at the start of each word.
* All rules must have a dot point.
* All dot points must be `*`, not `-`, or `+`.
* `Must` must be used instead of `should`.
* `These quotes` must be used where they look nice.
* `Look nice` must be used instead of `nice looking`.
* Lists in rules must have a `,` before the `and`, or `or`.
* Full stops must be used at the end of rules.
* `Especially` must be avoided.
* Characters must be referred to literally, except for full stops, dot points, tabs, and spaces.
* `Must be used` must be used instead of `is preferred`.
* `As` must be used instead of `as follows`, or `as the following`.

## Lua
* All tables possible must be sequential.
* All variables must be declared as `local`.
* Tabs must be used, not spaces.
* No variables should be declared such as `local math = math` unless in a module
* Spacing must remain consistent and look nice.
* Strings must use `"`, not `'`, unless `[[` and `]]` are required.
* `(` and `)` must not be used unless required.
* For indexed sequential tables, `ipairs` must be used, not `pairs`.
* Unused function return values must be set as `_`.
* Unused keys or values in a `for` loop must be set as `_`.
* `;` semicolons must never be used.
* Variable names must be in camelCase as well as functions.
* Variables must be named `str` instead of `txt`.
* Variables must not be the name of an existing object.
* `math.random( 1, n )` must be `math.random( n )`.
* To choose a random boolean, `math.random() > 0.5` is preferred.
* `While` and `until` loops must be avoided in favour of `for` loops.
* `math.randomseed` must never be called.

## Garry's Mod
* All repositories intended for external use must be structured as `GMod-INSERT-NAME`.
* All repositories must have tags of the following: `garrys-mod` `garrysmod` `garry-mod` `garrysmod-addon` `lua` `addon` `glua` `gmod` `gmod-lua`
* If the repository contains code for a STOOL, then `garrysmod-tool` must also be included.
* All repository descriptions must be structured as `INSERT NAME for Garry's Mod`.
* `AddCSLuaFile` must never be used for `lua/autorun` files.
* All repositories must include an addon `.jpeg`, `.jpg`, `.png`, and `.psd`.
* All repository `README` files must be structured as the following:

```
# Garry's Mod NAME
All the code for my NAME addon can be found here, and the actual addon is available [here](ADDON LINK).
![Icon](ICON PATH?raw=true)
```

## XCode
* All warnings must be enabled.
* The iOS requirement must be kept as low as possible.
* Warnings must be treated as errors.
* Projects must include a full icon set.
* All errors must be handled properly.

## Swift
* Variables must be declared as `private`, unless required by the compiler.
* Variable names must be American.
* No variables must be above the level of `internal`.
* `===` and `!==` are preferred over `==` and `!=`.
* No variables must be type declared, except for numbers.
* Variables must use `get`, `set`, and `didSet` where possible.
* `?` weak and `!` implicitly unwrapped variables must be avoided.
* Arrays are preferred over sets.
* All classes must be marked as `final` unless intended to be overwritten. If so, as many variables in the class as possible should be marked as `final`.
* Unused variables must be set as `_`.
* Structs must be used over classes where possible.
* `arc4random` and `arc4random_uniform` must be used for random number generation.
* `DispatchQueue` must be avoided.
* `SKShapeNode` must never be used, as it leaks memory.
* `UIBezierPath` must be avoided in favour of `CGPath`, as it is a wrapper.
* To remove an element from an array, `array = array.filter { $0 !== element }` is preferred.
* Extensions must be used to reduce namespace clutter.
* Variables must be marked as `let` unless the compiler requires `var`.
