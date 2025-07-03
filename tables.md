# Tables

To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate columns. For compatibility, add a pipe at both ends of the row.
You can align text left, right, or center by adding a colon (:) to the left, right, or both sides of the hyphens in the header row.

⚠️ You can’t use headings, blockquotes, lists, horizontal rules, images, or most HTML tags inside tables.
To display a pipe (|) in a table, use its HTML code (`&#124;`) because pipes are invisible in the rendered table.

```md
| Syntax | Description |
| ----------- | ----------- |  <!-- To underline headings -->
| Header | Title |
| Paragraph | Text |

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |  <!-- To align text -->
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

You can add a list inside a table cell by using HTML tags, because directly adding list elements (`*`, `-`, `+`) won't work. Same for `<br>` tags.

## Table of Contents

```md
- [Horizontal Rule](index.md#horizontal-rule-hr)  
- [Images](index.md#images)  
- [Links](index.md#links)
```

* [Horizontal Rule](index.md#horizontal-rule-hr)
* [Images](index.md#images)
* [Links](index.md#links)

# Works but Deprecated

## Center

Markdown has no direct way to center text, but HTML can be used:

```html
<center>This text is centered.</center>
```

<center>This text is centered.</center>

## Color

```html
<font color="red">This text is red!</font>
```

<font color="red">This text is red!</font>

# Comments

Here's a paragraph that will be visible.

[This is a comment that will be hidden.]: # 

And here's another paragraph that's visible.

# Symbols
Not supported by Markdown, but you can use HTML entities to display special characters or symbols.

Here’s a partial list of HTML entities for symbols:

Copyright (©) — &copy;
Registered trademark (®) — &reg;
Trademark (™) — &trade;
Euro (€) — &euro;
Left arrow (←) — &larr;
Up arrow (↑) — &uarr;
Right arrow (→) — &rarr;
Down arrow (↓) — &darr;
Degree (°) — &#176;
Pi (π) — &#960;

# Video

For embedding videos, you can use the following Markdown syntax. Replace `YOUTUBE-ID` with the actual ID of the YouTube video you want to embed.
`[![Image alt text](https://img.youtube.com/vi/YOUTUBE-ID/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE-ID)`
[![Less Than Jake — Scott Farcas Takes It On The Chin](https://img.youtube.com/vi/PYCxct2e0zI/0.jpg)](https://www.youtube.com/watch?v=PYCxct2e0zI)
