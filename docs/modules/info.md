# Info

This module brings informational pages.

The directory `info/` contains the info pages; if the directory does **not** exist, it will be created along 3 `.txt` files.

- `motd.txt`: this file contains the message of the day. This file is read when joining the server or when `/motd` is ran.
- `rules.txt`: this file contains the rules. This file is read when running `/rules`.
- `formatting.txt`: this file contains an example of the formatting used by Solstice. You can safely delete this file.

The files in `info/` support [Simplified Text Format](https://placeholders.pb4.eu/user/text-format/) and [Placeholders](https://placeholders.pb4.eu/user/default-placeholders/).

## Special pages

### Message of the day

The MOTD is displayed to a player whenever joining the server and with the `/motd` command. Uses the `motd.txt` file.

### Rules

Rules are displayed with the `/rules` command. Uses the `rules.txt` file.

## Configuration

### Enable MOTD - `enable-motd`

Whether to send the MOTD message when joining.

## Commands

- `/info` - Get a list of pages.
- `/info <page>` - Read page.
- `/motd` - Read MOTD.
- `/rules` - Read rules.