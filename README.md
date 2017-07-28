# MysteryPancake's Rule Book
## GitHub
* Editing code directly on this site mustn't occur (too often).
* Repository names must have capitals at the start of each word.
* Repository names must use `-` to separate words.
* Repository names must be as short as possible.
* Repository descriptions mustn't include a full stop.
* Repository descriptions must be as short as possible.
* Repositories intended for personal use must include an `MIT License` with `MysteryPancake` as the legal name.
* Repositories intended for external use mustn't include a license.
* Images in `README.md` files must be included in the repository, not on an external site.
* Small unused scripts must be added to [the Fun repository](https://github.com/MysteryPancake/Fun).

## Lua
* `If` statements in functions containing the rest of the code must instead `return end`.
* Boolean variables must be checked with `if bool then`, not `if bool == true then`.
* Expressions with the style of `x = x * 0.75` must be used, not `x = x - x / 4`.
* Strings must use `"`, not `'`, unless `[[` and `]]` are essential.
* `for` loops must be used, not `while`, `repeat` or `until` loops.
* `local var = var` mustn't be used, unless essential in a module.
* To check if a table is empty, `next(table) == nil` must be used.
* To choose a random boolean, `math.random() > 0.5` must be used.
* `math.random( 1, n )` must be shortened to `math.random( n )`.
* Generic string variables must be named `str`, not `txt`.
* Variables mustn't have the names of existing variables.
* To invert variables `-var` or `not var` must be used.
* Unused function return variables must be set as `_`.
* Unused keys or values in loops must be set as `_`.
* Sequential tables must be iterated with `ipairs`.
* `(` and `)` mustn't be used, unless essential.
* Tables must be sequential whenever possible.
* Tab indentation must be used, not spaces.
* Spaces must be on both sides of `..`.
* Spacing must be between everything.
* `math.randomseed` mustn't be used.
* Variables must be `local`.
* `;` mustn't be used.

## Garry's Mod
* Repositories intended for external use must be named with the style of `GMod-Insert-Name-Here`.
* Repositories must include the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod` and `gmod-lua`.
* Repositories for Scripted Tools must include the tag `garrysmod-tool`.
* Repository descriptions must have the style of `Insert Name Here for Garry's Mod`.
* Repositories must include an addon icon image, and the associated Photoshop file.
* Repositories must include a link to the addon.
* Repository `README.md` files must use the following style:

```
# Garry's Mod NAME
All the code for my NAME addon can be found here, and the actual addon is available [here](ADDON LINK).

![Icon](ICON PATH?raw=true)
```
* To add playermodels, `player_manager.AddValidModel( "Model Name", "models/player/model.mdl" )` must be used.
* Functions with applicable default arguments mustn't be called with the arguments.
* Variable names must be in `camelCase`, except for functions.
* `AddCSLuaFile` mustn't be used for files in `lua/autorun`.
* `and`, `or` and `not` must be used, not `&&`, `||` or `!`.
* `Panel` must be used, not `DPanel`.
* Hooks must use anonymous functions.

## XCode
* The iOS requirement must be kept as low as possible.
* Projects must include a complete icon set.
* All build warnings must be enabled.
* Warnings must be treated as errors.
* Errors must be handled safely.

## Swift
* Arrays with repeated variables must be initialized as `x: [Any] = Array(repeating: n, count: n)`, not `x = [Any](repeating: n, count: n)`.
* Dictionaries must be initialized as `x: [Any: Any] = [:]`, not `x = [Any: Any]()`.
* To generate random numbers, `arc4random` or `arc4random_uniform` must be used.
* A newline mustn't be before the closing `}` of classes, functions or structs.
* Expressions with the style of `x *= 0.75` must be used, not `x = x - x / 4`.
* Classes must be initialized as `final` unless intended to be overridden.
* When calling functions with specific arguments `.init` mustn't be used.
* Overridable classes must have as many `final` properties as possible.
* To join variables with strings, `"String \(variable)"` must be used.
* To invert variables, `-var` or `!var` must be used, not `var * -1`.
* Arrays must be initialized as `x: [Any] = []`, not `x = [Any]()`.
* When calling functions with specific arguments, `.` must be used.
* `for` loops must be used, not `while`, `repeat` or `until` loops.
* Division mustn't be used because it's slower than multiplication.
* `===` and `!==` must be used when possible, not `==` or `!=`.
* Variables mustn't be type declared, unless they're numbers.
* Variables must use `get`, `set` and `didSet` when possible.
* `struct` must be used, not `class`, unless essential.
* Extensions must be used to reduce namespace clutter.
* Variables mustn't be above the level of `internal`.
* Variables must be `let` unless `var` is essential.
* `SKShapeNode` mustn't be used, as it leaks memory.
* `Array` and `Dictionary` must be used, not `Set`.
* Double space indentation must be used, not tabs.
* `(` and `)` mustn't be used, unless essential.
* Ranges in `for` loops mustn't include spaces.
* `?` and `!` variables mustn't be used.
* Variable names must be in `camelCase`.
* Unused variables must be set as `_`.
* `DispatchQueue` mustn't be used.
* Variables must be `private`.
