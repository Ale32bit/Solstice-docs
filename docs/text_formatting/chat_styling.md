# Chat styling

## Advancements - `advancement-formats`

There are 3 kinds of advancements, called frames: **task**, **challenge**, **goal**.

![Advancements](../assets/text_formatting/advancements.png)

You can read more about them in the [Minecraft Wiki](https://minecraft.wiki/w/Advancement).

The advancement titles and descriptions are automatically translated to the client's locale.

- `${title}` - Title of the advancement.
- `${description}` - Description of the advancement.

## Player chat messages - `chat-format`

- `${message}` - The message content.

## Death messages - `death-format`

- `${message}` - The death message, it already contains the player name.

## Emote messages (`/me`) - `emote-format`

- `${message}` - The message content.

## Join message - `join-format`

- *No contextual placeholders*

## Join with a new username message - `join-renamed-format`

- `${previousName}` - Previous name of the player.

## Leave format - `leave-format`

- *No contextual placeholders*