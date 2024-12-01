# AutoAnnouncements

The automatic announcements module, as the name suggests, automatically broadcasts announcements to all players.

Single announcements can be configured to broadcast only to a subset of players that respect a configurable permission condition.

## Configuring

AutoAnnouncements can be configured in the `auto-announcements` section in the config file.

### Enable announcements - `enable-announcements`

Whether to enable automatic announcements.

### Delay - `delay`

Time in seconds to wait between each announcement.

### Pick randomly - `pick-randomly`

Whether to pick announcements in a random order instead of following the list order.

### Announcements - `announcements`

This list contains the each announcement available to broadcast.

Every entry must have a `text` parameter containing the message, if you wish to send the announcement only to a subset of players you can define the permission node and the result it must be.

!!! example

    If an announcement requires that the player has the permission node `allow.announcement`, the `result` parameter must be `true`.
    Else you can set `result` to `false` and it will only be sent to players that do **not** have that permission node set to `true`.

!!! warning

     Omitting the `permission` or `result` parameters will make it broadcast to everyone regardless.

```hocon
{
    text="Announcement Here!" # Announcement message

    # Optional. This parameter is the permission node to check on the player.
    permission="permission.node.here"

    # Optional. Result of the permission check. If it matches, it will be sent to the player.
    result=true 
}
```