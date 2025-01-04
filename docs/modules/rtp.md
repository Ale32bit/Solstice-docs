# RTP

This module adds the `/rtp` command to randomly warp to a location of the world.

## Configuration

!!! config "attempts"

    How many times to try to find a valid spot to teleport to before failing.

!!! config "timeout"

    How much time in milliseconds /rtp can take at most before failing.

!!! config "min-radius"

    Minimum radius from the center of the world border.

!!! config "max-radius"

    Maximum radius from the center of the world border. It caps to world border size.

!!! config "around-player"

    Use player as the center of the radius instead of the world border.

!!! config "prohibited-biomes"

    List of biomes an attempt should fail at.

!!! config "require-world-permission"

    Require that the player has the permission of the world `solstice.rtp.worlds.<worldName>` to initiate the random teleport in the world.

### Cooldown

!!! config "enable"

    This setting makes it so players have to wait before running the command a second time.

!!! config "cooldown"

    Seconds to wait for the cooldown to expire.

!!! config "cancel-on-fail"

    Cancel the cooldown if /rtp fails.

## Commands

!!! command "rtp"

    Warp to a random location of the world.

    **Permissions**

    * `solstice.rtp.base` - Default: 2
    * `solstice.rtp.worlds.<worldName>` - Default: 2<br>See `require-world-permission` setting.