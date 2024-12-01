# Chat Formatting

Solstice adds limited toggleable Markdown formatting to player chats.

Also you can replace chunks of text with something else.

## Configuring

These options can be configured in the `chat` section of the config file.

## Markdown

![Markdown](../assets/features/markdown.webp)

### Enable chat markdown - `enable-chat-markdown`

Whether to enable Markdown in chat.

### Format

The format allows:

- **bold** `**bold**`
- *italic* `*italic*`
- <u>underline</u> `__underline__`
- ~~strikethrough~~ `~~strikethrough~~`
- [Links](https://example.com) `[URLs](https://example.com)` (it shows original URL when hovering over it)
- `quotes` `` `quotes` ``
- ||spoilers|| `||spoilers||` (it shows text when hovering over it)

## Replacements - `replacements`

Chunks of texts can be replaced by configuring this key=value table.

You can add a replacement by adding a line like this to the list:

```hocon
"original"="replacement"
```