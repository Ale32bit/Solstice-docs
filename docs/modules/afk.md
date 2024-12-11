# AFK

The AFK (away-from-keyboard) module tracks players active time and automatically flags them as "AFK" after a configurable time span of inactivity.

The placeholder `solstice:afk` displays an AFK tag.

Activity is currently tracked by:

- Player movement
- Chat messages and commands
- Block and entity events
- Item use events

The `/afk` command manually triggers AFK.

![AFK](../assets/features/afk.png)

## Configuring

AFK can be configured in the `afk` section in the config file.

### Enable AFK - `enable`

Whether to enable the AFK module. This setting requires a server restart.

### AFK time trigger - `time-trigger`

How many seconds the player has to be inactive to trigger the AFK.

### Announce AFK - `announce`

Whether to announce in chat a player has gone to or returned from AFK.

### AFK Tag

This tag is displayed with `solstice:afk` placeholder when the player is AFK.

## Commands

- `/afk`