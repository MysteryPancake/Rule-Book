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
* `tbl[ math.random( #tbl ) ]` must be used to get a random value from a table.
* Strings must use `"`, not `'`, unless `[[` and `]]` are essential.
* `for` loops must be used, not `while`, `repeat` or `until` loops.
* `next(table) == nil` must be used to check if a table is empty.
* `math.random( 1, n )` must be shortened to `math.random( n )`.
* `math.random() > 0.5` must be used to get a random boolean.
* `if` statements containing lots of code must `return end`.
* Generic string variables must be named `str`, not `txt`.
* `if bool then` must be used, not `if bool == true then`.
* Variables mustn't have the names of existing variables.
* `local var = var` mustn't be used, unless for a module.
* `-var` or `not var` must be used to invert variables.
* Unused function return variables must be set as `_`.
* Unused keys or values in loops must be set as `_`.
* Sequential tables must be iterated with `ipairs`.
* Tables must be on a single line, unless wrapping.
* `x *= 0.75` must be used, not `x = x - x / 4`.
* `(` and `)` mustn't be used, unless essential.
* Metamethods mustn't be used unless essential.
* Tab indentation must be used, not spaces.
* Tables must be sequential when possible.
* Spaces must be on both sides of `..`.
* Spacing must be between everything.
* `math.randomseed` mustn't be used.
* `setmetatable` mustn't be used.
* Variables must be `local`.
* `;` mustn't be used.

## Garry's Mod
* Repositories intended for external use must be named `GMod-Insert-Name-Here`.
* Repositories must include the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod` and `gmod-lua`.
* Repositories for Scripted Tools must include the tag `garrysmod-tool`.
* Repository descriptions must be `Insert Name Here for Garry's Mod`.
* Repositories must include an addon icon image, and the associated Photoshop file.
* Repositories must include a link to the addon.
* Repository `README.md` files must use the following template:

```
# Garry's Mod NAME
All the code for my NAME addon can be found here, and the actual addon is available [here](ADDON LINK).

![Icon](ICON PATH?raw=true)
```
* `player_manager.AddValidModel( "Model Name", "models/player/model.mdl" )` must be used to add playermodels.
* Functions with applicable default arguments mustn't be called with the arguments.
* Functions with enum arguments mustn't be called with decimal values.
* Variable names must be in `camelCase`, except for functions.
* `AddCSLuaFile` mustn't be used for files in `lua/autorun`.
* `and`, `or` and `not` must be used, not `&&`, `||` or `!`.
* `if IsValid( obj ) then` must be used to validate objects.
* `Panel` must be used, not `DPanel`.
* Hooks must use anonymous functions.
* `table.Random` mustn't be used.

## XCode
* The iOS requirement must be kept as low as possible.
* Projects must include a complete icon set.
* All build warnings must be enabled.
* Warnings must be treated as errors.
* Errors must be handled safely.

## Swift
* Arrays with repeated variables must be `x: [Any] = Array(repeating: n, count: n)`, not `x = [Any](repeating: n, count: n)`.
* `arc4random_uniform(max - min) + min` must be used to get random numbers in a range.
* `UserDefaults.standard` must be used to save data such as scores and progress.
* `arc4random` or `arc4random_uniform` must be used to get random numbers.
* `.init` mustn't be used when calling functions with specific arguments.
* Overridable classes must have as many `final` properties as possible.
* `"String \(variable)"` must be used to join variables with strings.
* Dictionaries must be `x: [Any: Any] = [:]`, not `x = [Any: Any]()`.
* `-var` or `!var` must be used to invert variables, not `var * -1`.
* `for` loops must be used, not `while`, `repeat` or `until` loops.
* Division mustn't be used because it's slower than multiplication.
* `.` must be used when calling functions with specific arguments.
* Generic variables set as `SKAction.wait` must be named `delay`.
* Extensions and enums must be used to reduce namespace clutter.
* `===` and `!==` must be used when possible, not `==` or `!=`.
* Variables mustn't be type declared, unless they're numbers.
* Variables must use `get`, `set` and `didSet` when possible.
* `if` statements must be on a single line, unless wrapping.
* Classes must be `final` unless intended to be overridden.
* `if bool then` must be used, not `if bool == true then`.
* `struct` must be used, not `class`, unless essential.
* Variables mustn't be above the level of `internal`.
* Arrays must be `x: [Any] = []`, not `x = [Any]()`.
* Variables must be `let` unless `var` is essential.
* `SKShapeNode` mustn't be used, as it leaks memory.
* `Array` and `Dictionary` must be used, not `Set`.
* Double space indentation must be used, not tabs.
* `x *= 0.75` must be used, not `x = x - x / 4`.
* `(` and `)` mustn't be used, unless essential.
* Ranges in `for` loops mustn't include spaces.
* Unnecessary libraries mustn't be imported.
* `?` and `!` variables mustn't be used.
* Variable names must be in `camelCase`.
* Unused pointers must be set as `nil`.
* Unused variables must be set as `_`.
* `DispatchQueue` mustn't be used.
* A newline mustn't be before `}`.
* `&` must be used for pointers.
* Variables must be `private`.
* `UInt` mustn't be used.
