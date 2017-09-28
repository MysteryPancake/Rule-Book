# MysteryPancake's Rule Book
## GitHub
### General
* Editing code directly on this site mustn't occur (too often).
* Repository names must have capitals at the start of each word.
* Repository names must use `-` to separate words.
* Repository names must be as short as possible.
* Repository descriptions mustn't include a full stop.
* Repository descriptions must be as short as possible.
* Repositories intended for personal use must include an `MIT License` with `MysteryPancake` as the legal name.
* Repositories intended for external use mustn't include a license.
* Variables to insert must be named `<VARIABLE>`, not `INSERT_VARIABLE_HERE`.
* Images in `README` files must be included in the repository, not on an external site.
* [Commits closing issues must be named `resolved`, `fixes`, or `resolves`, followed by the issue number](https://help.github.com/articles/closing-issues-using-keywords).
* Small unused scripts must be added to the [Fun repository](https://github.com/MysteryPancake/Fun).

### GitHub Pages
* Repositories must include the tags `github-pages`, `github-page`, `github-io`, `html`, `css`, `javascript`, `github-api`, and all website keywords.

### Garry's Mod
* Repositories intended for external use must be named `GMod-<Addon-Name>`.
* Repositories must include the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod`, and `gmod-lua`.
* Repositories for Scripted Tools must include the tag `garrysmod-tool`.
* Repository descriptions must be `<Addon Name> for Garry's Mod`.
* Repositories must include an addon icon image and the associated Photoshop file.
* Repositories must include a link to the addon.
* Repository `README` files must use this template:

```
# Garry's Mod <Addon Name>
All the code for my <Addon Name> addon can be found here, and the actual addon is available [here](<WORKSHOP_LINK>).

![Icon](<ICON_PATH>?raw=true)
```

## Programming
### General
* Functions with applicable default arguments mustn't be called with the arguments.
* General `string` variables must be named `str`, not `txt`, or `text`.
* `-var` or `!var` must be used to invert variables, not `var * -1`.
* Functions with `enum` arguments mustn't be called with raw values.
* Literal collections must be on a single line unless wrapping.
* `if` statements must be on a single line unless wrapping.
* `if bool then` must be used, not `if bool == true then`.
* Variables mustn't share the names of existing variables.
* `return` early from functions containing lots of code.
* Unused variables must be set as `_`, or removed.
* `x *= 0.75` must be used, not `x = x - x / 4`.
* `Client-side` must be used, not `clientside`.
* `Server-side` must be used, not `serverside`.
* [Multiplication must be used, not division](https://stackoverflow.com/questions/226465).
* Validate, sanitize and escape user data.
* Variable names must be in `camelCase`.
* [`General` must be used, not `generic`](https://ell.stackexchange.com/questions/16224).
* No unnecessary variables in loops.
* Strings must use `"`, not `'`.
* Errors must be handled safely.
* No unnecessary `(` or `)`.
* No unnecessary variables.
* [`;` mustn't be used](https://stackoverflow.com/questions/16862337).

### Lua
* `tbl[ math.random( #tbl ) ]` must be used to get a random value from a table.
* Sequential tables must be iterated with `ipairs` or a numeric `for` loop.
* `next( table ) == nil` must be used to check if a string-table is empty.
* Variables must be `local` unless intended to be globally overridden.
* `#table == 0` must be used to check if an integer-table is empty.
* `math.random( 1, n )` must be shortened to `math.random( n )`.
* Strings in tables must be `tbl.string`, not `tbl[ "string" ]`.
* `math.random() >= 0.5` must be used to get a random boolean.
* Unused keys or values in loops must be set as `_`.
* General table variables must be named `tbl`.
* `not var` must be used to invert booleans.
* Tab indentation must be used, not spaces.
* Tables must be sequential where possible.
* Spaces must be on both sides of `..`.
* Spacing must be between everything.
* [No unnecessary `local var = var`](https://lua-users.org/wiki/OptimisingUsingLocalVariables).
* No unnecessary metamethods.
* [`module` mustn't be used](https://lua-users.org/wiki/LuaModuleFunctionCritiqued).
* `select` mustn't be used.

### Garry's Mod
* `player_manager.AddValidModel( "Model Name", "models/player/model.mdl" )` must be used to add playermodels.
* [`IsValid( var )` must be used for validation, not `var:IsValid()`](https://github.com/MysteryPancake/Rule-Book/issues/4).
* `and`, `or`, and `not` must be used, not `&&`, `||`, or `!`.
* `AddCSLuaFile` mustn't be used for files in `lua/autorun`.
* General player variables must be named `ply`, not `pl`.
* Assume data sent to the server has malicious intent.
* `CurTime` must be used for in-game events.
* `SysTime` must be used for benchmarking.
* `RealTime` must be used for HUD events.
* `Panel` must be used, not `DPanel`.
* Hooks must use anonymous functions.
* `table.Random` mustn't be used.
* `Material` must be cached.
* `SENT`s must use this template:
```
AddCSLuaFile()

ENT.Base = "base_entity"
ENT.Type = "anim"

ENT.Spawnable = true
ENT.AdminOnly = true
ENT.Editable = false

ENT.PrintName = "Entity Name"
ENT.Author = "MysteryPancake"
ENT.Purpose = "Entity purpose"
ENT.Instructions = "Entity instructions"
ENT.Category = "Entity category"
ENT.RenderGroup = RENDERGROUP_OPAQUE
```

### XCode
* The iOS requirement must be kept as low as possible.
* Projects must include a complete icon set.
* All build warnings must be enabled.
* Warnings must be treated as errors.

### Swift
* Repeating arrays must be `x: [Any] = Array(repeating: n, count: n)`, not `x = [Any](repeating: n, count: n)`.
* `arc4random_uniform(max - min) + min` must be used to get random numbers in a range.
* `UserDefaults.standard` must be used to save data such as scores and progress.
* `arc4random` or `arc4random_uniform` must be used to get random numbers.
* `.init` mustn't be used when calling functions with specific arguments.
* Variables must be `private` unless intended to be globally overridden.
* [Overridable classes must have as many `final` properties as possible](https://stackoverflow.com/questions/35818703).
* `"String \(variable)"` must be used to join variables with strings.
* Dictionaries must be `x: [Any: Any] = [:]`, not `x = [Any: Any]()`.
* `.` must be used when calling functions with specific arguments.
* Extensions and enums must be used to reduce namespace clutter.
* Variables must use `get`, `set`, and `didSet` where possible.
* Variables mustn't be type declared unless they're numbers.
* Classes must be `final` unless intended to be overridden.
* General `SKAction.wait` variables must be named `delay`.
* `struct` must be used, not `class`, where possible.
* Variables mustn't be above the level of `internal`.
* Arrays must be `x: [Any] = []`, not `x = [Any]()`.
* `SKShapeNode` mustn't be used as it leaks memory.
* `Array` or `Dictionary` must be used, not `Set`.
* Double space indentation must be used, not tabs.
* `let` must be used unless `var` is essential.
* Ranges in `for` loops mustn't include spaces.
* `===` and `!==` must be used where possible.
* Unnecessary libraries mustn't be imported.
* `&&` must be used unless `,` is essential.
* `?` and `!` variables mustn't be used.
* Unused pointers must be set as `nil`.
* `DispatchQueue` mustn't be used.
* A newline mustn't be before `}`.
* [`Int` must be used, not `UInt`](https://stackoverflow.com/questions/24180630).
* `&` must be used for pointers.

### HTML
[This template](https://validator.w3.org) [must be used](https://gethead.info):
```
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8">
		<title>Title</title>
		<meta name="description" content="Description">
		<meta name="keywords" content="Key, Words">
		<meta property="og:title" content="Title">
		<meta property="og:type" content="website">
		<meta property="og:url" content="https://url.com">
		<meta property="og:image" content="https://url.com/image.png">
		<meta property="og:site_name" content="Title">
		<meta property="og:description" content="Description">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="stylesheet" type="text/css" href="style.css">
		<script async src="script.js"></script>
	</head>
	<body>
		<p>Content</p>
	</body>
</html>
```

### CSS
* [`body, html { background-color: white; }` must be used](https://stackoverflow.com/questions/35205683).
* [Hex colors must be uppercase](https://stackoverflow.com/questions/32695983).
* Alphabetize declarations.

### JavaScript
* `haystack.indexOf(needle) !== -1;` must be used to check if a string contains a substring.
* [Objects must have spacing `{ like: this }`](https://github.com/airbnb/javascript).
* [`XMLHttpRequest` must be asynchronous](https://blogs.msdn.microsoft.com/wer/2011/08/03/why-you-should-use-xmlhttprequest-asynchronously).
* [Always `"use strict";`](https://stackoverflow.com/a/1335881).
* [`var` must be used](https://stackoverflow.com/questions/22603078).
