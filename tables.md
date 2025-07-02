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
