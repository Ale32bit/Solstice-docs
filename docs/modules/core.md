# Core

This module adds core functionality shared between modules and updates players data.

## Configuration

### Date and time format

Some messages may include a date, a time or both.

You can use this [list of patterns](https://docs.oracle.com/javase/8/docs/api/java/time/format/DateTimeFormatter.html#patterns) to customize the formats.

#### Date format - `date-format`

- Metric: `dd/MM/yyyy`
- USA: `MM-dd-yyyy`

#### Time format - `time-format`

- 24h: `HH:mm`
- 12h: `hh:mm a`

#### Date & time format - `date-time-format`

*Combination of the above.*

### Links and URLs

You can customize how links are styled in chat.

These formats apply to both the Markdown link style (`[label](url)`) and URLs (`https://example.com`).

#### Link format - `link`

- `${label}` - Label of the link, will be URL if not in Markdown style.
  
#### Link hover format - `link-hover`

This format is displayed when hovering hover the link.

- `${url}` - URL of the link.

## Commands

- `/solstice`
- `/soltice reload` - (`solstice.command.solstice.reload`) - Reload configuration and locale files.