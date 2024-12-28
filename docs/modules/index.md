---
title: Introduction
---

# Modules

Modules bring functionalities and commands to Solstice.

Check out the left side bar for a list of documented modules.

## Default permission values

All permissions hold a default value when the permission check returns a non-existant value (is not set).

If the default value is `true`, the permission is granted to everyone, if it's `false` then the permission is denied by default to everyone.

If the value is a number between 0 and 4 (included), it references the operator [permission level](https://minecraft.wiki/w/Permission_level), useful when **LuckPerms** is not installed.

## Command arguments

Many commands hold arguments in the format of &lt;arg&gt; and [arg].

* `<arg>` - The argument is required.
* `[arg]` - The argument is optional.