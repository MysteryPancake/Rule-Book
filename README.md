# GitHub Rule Book
**The following rules must be obeyed under all circumstances.**
- All repository titles must have capital letters at the start of each word.
- All repository titles must have - dashes in place of spaces.
- All repositories intended for personal use must have an MIT license with MysteryPancake as the legal name. Otherwise, no license must be included.
- All repository descriptions must not include a full stop.
- Small pieces of code should be created in the Fun repository.

## Lua
- Tabs must be used, not spaces.
- No variables should be declared as such unless in a module: `local math = math`
- Spacing must remain consistent and nice looking.
- Strings must use `"` quotations, not `'`. If necessary, `[[` and `]]` brackets must be used.
- ( and ) parenthesis should be kept to a minimum unless required.
- For indexed sequential tables, `ipairs` should be used, not `pairs`.
- Unused function return values must be set as `_`.
- Unused keys or values in a for loop must be set as `_`.
- No `;` semicolons should be used, ever.
- Variable names must be in camelCase as well as functions.
- Variables should be named `str` instead of `txt`.
- Variables should not be the name of an existing object.
- `math.random( 1, n )` should be `math.random( n )`.
- To choose a random boolean, `math.random() > 0.5` is preferred.
- For loops are preferred over while and until loops.
- `math.randomseed` should never be called.

## Garry's Mod
- All repositories intended for external use must be structured as the following:

`GMod-NAME`

- All repositories must have tags of the following:

`garrys-mod` `garrysmod` `garry-mod` `garrysmod-addon` `lua` `addon` `glua` `gmod` `gmod-lua`

- All repository descriptions must be structured as the following:

`NAME for Garry's Mod`

- No `AddCSLuaFile` is to be used for `lua/autorun` files.
- All repositories must include an addon JPEG or PNG, as well as the PSD.
- All repository README files must be structured as the following:

```
# Garry's Mod NAME
All the code for my NAME addon can be found here, and the actual addon is available [here](ADDON LINK).
![Icon](ICON PATH?raw=true)
```

## Swift
- All variables possible should be kept `private`.
- No variables should be above the level of `internal`.
- No variables should be type declared, except for numbers.
- As few variables as possible should be weak or implicitly unwrapped.
- Arrays are preferred over sets.
- All classes must be marked as `final` unless intended to be overwritten. If so, as many variables in the class as possible should be marked as `final`.
- Unused variables must be set as `_`.
