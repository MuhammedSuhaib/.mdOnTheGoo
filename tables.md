
# Tables
To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate each column. For compatibility, you should also add a pipe on either end of the row.
You can align text in the columns to the left, right, or center by adding a colon (:) to the left, right, or on both side of the hyphens within the header row.

! You can’t use headings, blockquotes, lists, horizontal rules, images, or most HTML tags.
You can display a pipe (|) character in a table by using its HTML character code (&#124;). bcz pipes are invisible in the rendered table.


```md
| Syntax | Description |
| ----------- | ----------- | -----> To dark underline headings
| Header | Title |
| Paragraph | Text |

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: | ----->To align text
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

| Syntax | Description |
| ----------- | ----------- |
| Header | Title  |
| Paragraph | Text |



You can add a list within a table cell by using HTML tags. bcz directly adding a list elements (`*/-/+`) will not work. same for <br>

## Table of Contents

```
- [Horizontal Rule](index.md#horizontal-rule-hr)  
- [Images](index.md#images)  
- [Links](index.md#links)

```
- [Horizontal Rule](index.md#horizontal-rule-hr)  
- [Images](index.md#images)  
- [Links](index.md#links)


# Works but Depricated 

## Center

well there is no direct way to center text in markdown, but you can use HTML tags to achieve this.

```html

<center>This text is centered.</center>
```
<center>This text is centered.</center>
 
## Color
<font color="red">This text is red!</font>
```html
<font color="red">This text is red!</font>  
```