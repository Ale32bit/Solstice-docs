# Home

The home module brings player home waypoints.

## Configuration

!!! config "maxHomes"

    Maximum amount of homes a player can have.

    Set to `-1` to disable this limit.

## Commands

!!! command "home [name]"

    Warp to a home.

    The argument `name` defaults to `"home"`.

    **Permissions**

    * `solstice.home.base` - Default: true

!!! command "sethome [home] [force]"

    Set a home.

    The argument `name` defaults to `"home"`.

    The argument `force` is to be used when overriding an existing home.

    **Permissions**

    * `solstice.home.base` - Default: true

!!! command "delhome [name]"

    Delete a home.

    The argument `name` defaults to `"home"`.

    **Permissions**

    * `solstice.home.base` - Default: true

!!! command "homes [player]"

    List homes.

    **Permissions**

    * `solstice.home.base` - Default: true
    * `solstice.home.others` - Default: 2<br>Allows the use of the `player` argument to list a player's homes.

!!! command "homeother &lt;player&gt; [name]"

    Teleport to a player's home.

    The argument `name` defaults to `"home"`.

    **Permissions**

    * `solstice.home.others` - Defaults: 2