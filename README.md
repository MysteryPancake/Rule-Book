# Rule Book
## GitHub
* Editing on the site must be avoided, except for this file.
* Repo titles must have capital letters at the start of each word.
* Repo titles must have `-` instead of spaces.
* Repos intended for personal use must have an `MIT License` with `MysteryPancake` as the legal name. Otherwise, no license must be included.
* Repo descriptions must be as short as possible.
* Repo descriptions must not include a full stop.
* Small pieces of code must be added to the Fun repo.
* Images in the repo's `README` must be hosted on the repo, not an external site.

## Lua
* Tables must be sequential where possible.
* Variables must be declared as `local`.
* Tabs must be used, not spaces.
* No variables must be declared as `local var = var`, unless in a module.
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
* To choose a random boolean, `math.random() > 0.5` must be used.
* `While` and `until` loops must be avoided in favour of `for` loops.
* `math.randomseed` must not be used.

## Garry's Mod
* Repos intended for external use must be structured as `GMod-Insert-Name-Here`.
* Repos must have the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod`, and `gmod-lua`.
* If the repo is for a STOOL, then the tag `garrysmod-tool` must also be included.
* Repo descriptions must be structured as `Insert Name Here for Garry's Mod`.
* `AddCSLuaFile` must never be used for `lua/autorun` files.
* Repos must include an addon `.jpeg`, `.jpg`, `.png`, and `.psd`.
* Repo `README` files must be structured as the following:

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
* Errors must be handled properly.

## Swift
* Variables must be declared as `private`, unless required by the compiler.
* Variable names must be American.
* No variables must be above the level of `internal`.
* `===` and `!==` are preferred over `==` and `!=`.
* No variables must be type declared, except for numbers.
* Variables must use `get`, `set`, and `didSet` where possible.
* `?` weak and `!` implicitly unwrapped variables must be avoided.
* Arrays are preferred over sets.
* Classes must be marked as `final` unless intended to be overwritten. If so, as many variables in the class as possible should be marked as `final`.
* Unused variables must be set as `_`.
* Structs must be used over classes where possible.
* `arc4random` and `arc4random_uniform` must be used for random number generation.
* `DispatchQueue` must be avoided.
* `SKShapeNode` must never be used, as it leaks memory.
* `UIBezierPath` must be avoided in favour of `CGPath`, as it is a wrapper.
* To remove an element from an array, `array = array.filter { $0 !== element }` must be used.
* Extensions must be used to reduce namespace clutter.
* Variables must be marked as `let` unless the compiler requires `var`.
