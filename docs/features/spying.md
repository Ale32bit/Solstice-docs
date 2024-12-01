# Spying

## Social spy

Administrators can spy direct messages between players (and server) by granting the `solstice.tell.spy` permission.

### Configuring

The format can be changed in the `locale.json` file, on the `messageSpy` line under the `commands.tell` section.

#### Placeholders

- `${sourcePlayer}` - Player name that sent the message.
- `${targetPlayer}` - Player that received the message.
- `${message}` - The message.

## Command spy

Administrators can read every command executed by players (even failing ones) by granting the `solstice.commandspy` permission.

### Configuring

Command spy can be configured in the `command-spy` section of the config file.

#### Format - `command-spy-format`

The format to use when sending command spy notifications.

##### Placeholders

- `${player}` - Name of the player that sent the command.
- `${command}` - Full command, without `/`.

#### Ignored commands - `ignored-commands`

This list contains the commands to ignore.