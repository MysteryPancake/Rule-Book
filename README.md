# MysteryPancake's Rule Book
Please don't use this rule book. The rules are extremely arbitrary and change all the time.

It's a journal to help me try to remain consistent. It also helps me spot and fix common mistakes.

## GitHub
### Generic
* Repositories must have `README` files.
* Editing code directly on this site mustn't occur (too often).
* Repository names must be capitalized.
* Repository names must be as short as possible.
* Repository names must use `-` to separate words.
* Repository descriptions mustn't include a full stop.
* Repository descriptions must be as short as possible.
* Repositories intended for personal use must include an `MIT License` with `MysteryPancake` as the legal name.
* Repositories intended for external use must include an `Unlicense`.
* Variables to insert must be named `<VAR>`, not `INSERT_VAR_HERE`.
* Images in `README` files must be included in the repository, not on an external site.
* [Commits closing issues must be named `resolved`, `fixes`, or `resolves`, followed by the issue number](https://help.github.com/articles/closing-issues-using-keywords).
* [Small unused scripts must be added to the Fun repository](https://github.com/MysteryPancake/Fun).

### Garry's Mod
* Repositories intended for external use must be named `GMod-<Addon-Name>`.
* Repositories must include the tags `garrys-mod`, `garrysmod`, `garry-mod`, `garrysmod-addon`, `lua`, `addon`, `glua`, `gmod`, and `gmod-lua`.
* Repositories for Scripted Tools must include the tag `garrysmod-tool`.
* Repository descriptions must be `<Addon Name> for Garry's Mod`.
* Repositories must include an addon icon and the associated Photoshop file.
* Repositories must include a link to the addon.
* Repository `README` files must use this template:
```
<img src="<ICON_PATH>?raw=true" width="75" align="left">

# Garry's Mod <Addon Name>
All the code for my <Addon Name> addon can be found here, and the actual addon is available [here](<WORKSHOP_LINK>).
```

### Discord
* Repositories must include the tags `discord`, `discord-bot`, `discord-js`, `discord-api`, `discordjs`, `discordjs-bot`, `javascript`, `discordjsbot`, `discordapp`, `discordbot`, `nodejs-bot`, `nodejs`, `node-js`, and `bot`.
* Repositories must include a `Procfile` containing `worker: npm start`.
* Repository `README` files must include setup instructions.
* Repository `README` files must include a command list.
* Repositories must include a bot icon.
* Repository `package.json` files must use this template:
```
{
  "name": "<Repository-Name>",
  "version": "1.0.0",
  "description": "<Repository Description>",
  "main": "<SCRIPT_PATH>",
  "engines": {
    "node": "10.x",
    "npm": "*"
  },
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "node <SCRIPT_PATH>"
  },
  "keywords": [
    "discord",
    "discord-bot",
    "discord-js",
    "discord-api",
    "discordjs",
    "discordjs-bot",
    "javascript",
    "discordjsbot",
    "discordapp",
    "discordbot",
    "nodejs-bot",
    "nodejs",
    "node-js",
    "bot",
  ],
  "author": "MysteryPancake",
  "license": "MIT",
  "dependencies": {
    "discord.js": "<VERSION>"
  }
}
```

### GitHub Pages
* Repositories must include the tags `github-pages`, `github-page`, `github-io`, `html`, `css`, `javascript`, `github-api`, `website`, `online`, and all website keywords.
* Website links must have lowercase domains.
* Website links mustn't have a `/` at the end.
* Repositories must include a website link.

## Programming
### Generic
* Functions with applicable default arguments mustn't be called with the arguments.
* `while (lines.length > 0)` must be used, not `while (lines.length)`.
* Generic `string` variables must be named `str`, not `txt`, or `text`.
* `-foo` and `!foo` must be used to invert variables, not `foo * -1`.
* Functions with `enum` arguments mustn't be called with raw values.
* Literal collections must be on a single line unless wrapping.
* `if` statements must be on a single line unless wrapping.
* `if bool then` must be used, not `if bool == true then`.
* Variables mustn't share the names of existing variables.
* [The last condition of `switch` statements must `break`](https://stackoverflow.com/a/26139061).
* `return` early from functions containing lots of code.
* Functions mustn't have unintentional side effects.
* [`application/xml` must be used, not `text/xml`](https://stackoverflow.com/a/6141983).
* [`switch` statements mustn't have additional tabs](https://stackoverflow.com/a/3005855).
* Unused variables must be set as `_`, or removed.
* `x *= 0.75` must be used, not `x = x - x / 4`.
* `Clientside` must be used, not `client-side`.
* `Serverside` must be used, not `server-side`.
* [Multiplication must be used, not division](https://stackoverflow.com/questions/226465).
* Powers of two must be used where possible.
* Triple newlines `\n\n\n` mustn't be used.
* Validate, sanitize and escape user data.
* Variable names must be in `camelCase`.
* [`Generic` must be used, not `general`](https://ell.stackexchange.com/a/16225).
* No unnecessary variables in loops.
* `Setup` must be used, not `init`.
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
* Unused keys and values in loops must be set as `_`.
* Generic table variables must be named `tbl`.
* `return end` must be followed by a newline.
* `not foo` must be used to invert booleans.
* Tab indentation must be used, not spaces.
* Tables must be sequential where possible.
* `return` must be used, not `return nil`.
* Spaces must be on both sides of `..`.
* Spacing must be between everything.
* `local foo = foo` mustn't be used.
* No unnecessary metamethods.
* [`module` mustn't be used](https://lua-users.org/wiki/LuaModuleFunctionCritiqued).
* `select` mustn't be used.

### Garry's Mod
* `player_manager.AddValidModel( "Model Name", "models/player/model.mdl" )` must be used to add playermodels.
* `foo:BoundingRadius()` must be used, not `foo:OBBMins():Distance( foo:OBBMaxs() )`.
* `tobool( foo:GetInfo( "bar" ) )` must be used to check a ConVar as a bool.
* In `PlayerSay` and `OnPlayerChat`, `text` must be used, not `txt` or `str`.
* `foo:GetInfo( "bar" )` must be used, not `foo:GetInfoNum( "bar" )`.
* [`IsValid( foo )` must be used for validation, not `foo:IsValid()`](https://github.com/MysteryPancake/Rule-Book/issues/4).
* [`player.GetHumans()` must be used, not `player.GetAll()`](https://wiki.garrysmod.com/page/player/GetHumans).
* `AddCSLuaFile` mustn't be used for files in `lua/autorun`.
* [`or`, `and`, `not`, `~=`, `--[[ ]]` and `--` must be used](https://wiki.garrysmod.com/page/Specific_Operators).
* Generic player variables must be named `ply`, not `pl`.
* Assume data sent to the server has malicious intent.
* [`self:GetOwner()` must be used, not `self.Owner`](https://github.com/Facepunch/garrysmod/pull/1417).
* [`SOLID_OBB` must be used, not `SOLID_BBOX`](https://facepunch.com/showthread.php?t=1548067&p=52780912&viewfull=1#post52780912).
* Hooks must be added in `lua/autorun` files.
* `CurTime` must be used for in-game events.
* `SysTime` must be used for benchmarking.
* `RealTime` must be used for HUD events.
* `Panel` must be used, not `DPanel`.
* [`foo:PhysWake()` must be used](https://wiki.garrysmod.com/page/Entity/PhysWake).
* `table.Random` mustn't be used.
* `Material` must be cached.
* `SENT`s must use this template:
```
AddCSLuaFile()

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
* `arc4random` and `arc4random_uniform` must be used to get random numbers.
* `.init` mustn't be used when calling functions with specific arguments.
* Variables must be `private` unless intended to be globally overridden.
* [Overridable classes must have as many `final` properties as possible](https://stackoverflow.com/questions/35818703).
* Dictionaries must be `x: [Any: Any] = [:]`, not `x = [Any: Any]()`.
* `.` must be used when calling functions with specific arguments.
* Extensions and enums must be used to reduce namespace clutter.
* `"String \(foo)"` must be used to join variables with strings.
* Variables must use `get`, `set`, and `didSet` where possible.
* Variables mustn't be type declared unless they're numbers.
* Classes must be `final` unless intended to be overridden.
* Generic `SKAction.wait` variables must be named `delay`.
* `struct` must be used, not `class`, where possible.
* Variables mustn't be above the level of `internal`.
* Arrays must be `x: [Any] = []`, not `x = [Any]()`.
* `Array` and `Dictionary` must be used, not `Set`.
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
* [`SKShapeNode` mustn't be used](http://sartak.org/2014/03/skshapenode-you-are-dead-to-me.html).
* [`Int` must be used, not `UInt`](https://stackoverflow.com/questions/24180630).
* `&` must be used for pointers.

### HTML
[This template](https://validator.w3.org) [must be used](https://gethead.info):
```
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8">
		<title><Repository Name></title>
		<meta name="description" content="<Repository Description>">
		<meta name="keywords" content="<Repository, Key, Words>">
		<meta property="og:title" content="<Repository Title>">
		<meta property="og:type" content="website">
		<meta property="og:url" content="<WEBSITE_URL>">
		<meta property="og:image" content="<ICON_PATH>">
		<meta property="og:site_name" content="<Repository Title>">
		<meta property="og:description" content="<Repository Description>">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="stylesheet" type="text/css" href="style.css">
		<script src="script.js"></script>
	</head>
	<body>
		<span>Content</span>
	</body>
</html>
```
* [To improve responsiveness, `onmousedown` must be used instead of `onclick` where possible](https://hackernoon.com/instant-actions-onmousedown-vs-onclick-37f20b00eaf0).
* [CSS must be used for sizing iframes, not `<iframe width=<WIDTH> height=<HEIGHT>`](https://benmarshall.me/responsive-iframes).
* [`<script>` must be used, not `<script type="text/javascript">`](https://stackoverflow.com/a/4243934).
* [`<style>` must be used, not `<style type="text/css">`](https://forum.webflow.com/t/style-vs-style-type-text-css/10685/2).
* [`async` and `defer` must be used carefully](https://stackoverflow.com/a/44443936).
* [Attributes must be quoted](https://stackoverflow.com/a/6495345).
* Alphabetize keywords.

### CSS
* [`font-size: small` and `font-size: large` must be used, not `font-size: smaller` or `font-size:larger`](https://www.w3schools.com/cssref/pr_font_font-size.asp).
* [`-moz-user-select: none` must be used alongside `user-select: none`](https://developer.mozilla.org/en-US/docs/Web/CSS/user-select).
* [Box shadows must be used for inset borders](https://stackoverflow.com/a/8452798).
* [Hex colors must be uppercase](https://stackoverflow.com/questions/32695983).
* [Use `outline: none` sparingly](http://www.outlinenone.com).
* Alphabetize declarations.

### JavaScript
* [`encodeURIComponent` and `decodeURIComponent` must be used, not `encodeURI` or `decodeURI`](https://stackoverflow.com/a/747700).
* [`haystack.indexOf(needle) !== -1;` must be used to check if a string contains a substring](https://jsperf.com/exec-vs-match-vs-test-vs-search).
* [`.split("str")[0]` must be used to get text before a string, not `.split("str").shift()`](https://stackoverflow.com/a/33437745).
* `foo += bar` and `foo -= bar` must be used, not `foo = foo + bar` or `foo = foo - bar`.
* [`window.innerWidth` and `window.innerHeight` must be used to get the document size](https://www.w3schools.com/jsref/prop_win_innerheight.asp).
* Javascript names mustn't be used in objects: `{ "false": true }[false] -> true`
* [`if (array.length) {` must be used, not `if (array.length > 0) {`](https://stackoverflow.com/a/32911903).
* `foo++` and `foo--` must be used, not `foo += 1` or `foo -= 1`.
* [`responseText` and `responseXML` must be used, not `response`](https://stackoverflow.com/a/46751655).
* [`console.error` must be used to log errors, not `console.log`](https://stackoverflow.com/a/25532848).
* [`str.replace(/\.[^/.]+$/, "")` must be used to get a file name](https://stackoverflow.com/a/4250408).
* [`str.split(".").pop()` must be used to get a file extension](https://stackoverflow.com/a/190878).
* [`string.charAt` must be used to get a character in a string](https://stackoverflow.com/a/3427148).
* [`textContent` must be used, unless `innerHTML` is essential.](https://stackoverflow.com/a/21311670).
* `bool ? foo : bar` must be used, not `bool && foo || bar`.
* `window.` must be before `window` methods and properties.
* Global variables must be declared at the top of the script.
* [`style.display = none` must be used, not `removeChild`](https://stackoverflow.com/a/2457637).
* [`parseInt` and `parseFloat` must be used, not `Number`](https://stackoverflow.com/a/1133780).
* [Function arguments must have spacing `(like, this)`](https://github.com/airbnb/javascript).
* [`parentNode` must be used, not `parentElement`](https://stackoverflow.com/a/8685780).
* [`textContent` must be used, not `innerText`](https://stackoverflow.com/a/35213204).
* [`const` must be used for arrays and objects](https://mathiasbynens.be/notes/es6-const).
* [Objects must have spacing `{ like: this }`](https://github.com/airbnb/javascript).
* [Asynchronous callbacks must use promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises#Guarantees).
* [`childNodes` must be used, not `children`](https://stackoverflow.com/a/7935719).
* [Canvas contexts must have alpha disabled](https://webglfundamentals.org/webgl/lessons/webgl-and-alpha.html).
* [`&&`, `!`, and `||` must be used carefully](https://github.com/airbnb/javascript/pull/590).
* [`.toString()` must be used, not `String`](https://stackoverflow.com/a/5765406).
* [`"property" in window` mustn't be used](http://2ality.com/2013/09/window.html).
* [`XMLHttpRequest` must be asynchronous](https://blogs.msdn.microsoft.com/wer/2011/08/03/why-you-should-use-xmlhttprequest-asynchronously).
* [`keydown` must be used, not `keypress`](https://www.mutuallyhuman.com/blog/keydown-is-the-only-keyboard-event-we-need).
* [`wheel` must be used, not `mousewheel`](https://developer.mozilla.org/en-US/docs/Web/Events/mousewheel).
* [`initial` must be used, not `origin`](https://www.w3schools.com/jsref/prop_loc_origin.asp).
* [`for` must be used, not `forEach`](https://coderwall.com/p/kvzbpa/don-t-use-array-foreach-use-for-instead).
* [Constructors must be capitalized](https://stackoverflow.com/a/1564489).
* `Object.keys()` mustn't be used.
* [`\"` must be used, not `'`](https://stackoverflow.com/a/2004178).
* [No use before define](https://eslint.org/docs/rules/no-use-before-define).
* `` ` `` mustn't be used.
* [`;` must be used](https://stackoverflow.com/a/444082).
* [This must be used to remove an element from an array](https://stackoverflow.com/a/5767357):
```
var index = array.indexOf(foo);
if (index !== -1) {
	array.splice(index, 1);
}
```

### Unity
* Class functions must be sorted by `Awake`, `Start`, `Update`, `FixedUpdate`, `OnCollisionEnter`, `OnCollisionStay`, `OnCollisionExit`, `OnTriggerEnter`, `OnTriggerStay`, `OnTriggerExit`, and `OnBecameInvisible`.
* [`rigid2D.simulated = false` must be used to disable a `Rigidbody2D`, not `isKinematic = true`, or `Sleep()`](https://docs.unity3d.com/ScriptReference/Rigidbody2D-simulated.html).
* [`localPosition`, `localRotation`, and `localScale` must be used, unless `position` or `rotation` are essential](https://twitter.com/devangerist/status/1069501290026287104).
* For 2D games, `Vector2` must be used where possible, unless `Vector3` is essential.
* Class variables must be sorted by `internal`, `public`, then `private`.
* Variables not intended to be set in the editor must be `internal`.
* Class functions must be sorted by accessibility levels.
* [`sqrMagnitude` must be used when comparing vectors](https://docs.unity3d.com/ScriptReference/Vector2-sqrMagnitude.html).
* [`override` must be placed after the access modifier](https://unity3d.com/learn/tutorials/topics/scripting/overriding).
* [`Time.time > last` must only be used for delays](https://answers.unity.com/questions/890258/have-a-delay-after-each-jump-so-user-cant-spam-jum.html).
* [String switches must be used, not enum switches](https://stackoverflow.com/a/1947901).
* [`Awake` must be used, unless `Start` is essential](https://answers.unity.com/questions/382658/use-of-awake-vs-start.html).
* [`Time.deltaTime` must only be used for timers](https://answers.unity.com/questions/225213/c-countdown-timer.html).
* [`StartCoroutine`](https://docs.unity3d.com/ScriptReference/MonoBehaviour.StartCoroutine.html) must be used, not [`Invoke`](https://docs.unity3d.com/ScriptReference/MonoBehaviour.Invoke.html).
* `int` must be used, unless `float` is essential.
* [Animation layers must be used, not animators](https://docs.unity3d.com/Manual/AnimationLayers.html).
* [`StartsWith` and `EndsWith` mustn't be used](https://docs.unity3d.com/Manual/BestPracticeUnderstandingPerformanceInUnity5.html).
* [Variables must be as inaccessible as possible](https://stackoverflow.com/a/1295997).
* [Variables must be `private` where possible](https://stackoverflow.com/a/7385005).
* Animations mustn't affect enabled states.
* [`for` must be used, not `foreach`](https://forum.unity.com/threads/is-foreach-still-bad-for-performance.434782/).
* [Floats must be followed by `f`](https://stackoverflow.com/a/11590321).
* [`GetComponent` must be cached](https://unity3d.com/learn/tutorials/topics/performance-optimization/optimizing-scripts-unity-games).
* [Coroutines must be cached](https://twitter.com/bivolt_studio/status/1066695127995990016).

### GitHub Pages
* `window.alert` must be used for important errors, not `console.warn` or `console.log`.
* [Strings must be concatenated with `"foo" + bar`, not `"foo${bar}"`](https://stackoverflow.com/a/16124072).
* [Always `"use strict";`](https://stackoverflow.com/a/1335881).
