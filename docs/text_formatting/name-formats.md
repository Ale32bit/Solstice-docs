# Player name formats

It is possible to customize how player names are displayed in the server based on the LuckPerms group of the player.

!!! info

    If LuckPerms is not installed, or it is not possible to guess the group, Solstice falls back to two group names:

    - `default` - Used for everyone.
    - `operator` - Used by operators.

## Configure player names

Display names are configurable in the `name-formats` list.

This list uses the order as priority of the group, first elements come before later elements.

!!! example

    If the player is in the `vip` and `default` groups, but is not in the `admin` group, it will pick the `vip` group and skip `default` as `vip` comes before `default`.

    - admin
    - vip
    - default

### Adding a format

To add a format for a group, add the following lines in the list (remember the order priority in the list):

```hocon
{
    format="<blue>${name}</blue>" # Name format here
    group="mygroup" # Group name
}
```

#### Placeholder

Instead of using `%player:name%`, `${name}` is prefered because it respects the nickname of the player (if any).