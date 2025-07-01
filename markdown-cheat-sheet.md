# Markdown Cheat Sheet

Thanks for visiting [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for [basic syntax](https://www.markdownguide.org/basic-syntax/) and [extended syntax](https://www.markdownguide.org/extended-syntax/).

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

### Heading

# H1
## H2
### H3

### Bold

**bold text**

### Italic

*italicized text*

### Blockquote

> blockquote

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item

### Code

`code`

### Horizontal Rule

---

### Link

[Markdown Guide](https://www.markdownguide.org)

### Image

![alt text](https://www.markdownguide.org/assets/images/tux.png)

## Extended Syntax Working on github

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

```md
| Syntax | Description |
| ----------- | ----------- | -----> To dark underline headings
| Header | Title |
| Paragraph | Text |
```

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |



You can add a list within a table cell by using HTML tags. bcz directly adding a list elements (`*/-/+`) will not work.

#### Table of Contents

- [Underline](#underline)
- [Indent](#indent)
- [Center](#center)
- [Color](#color)

### Fenced Code Block (Language-specific code block)
code block with syntax highlighting colors etc

```py
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote (not supported in VS Code)
Footnotes create a reference link that takes you to a note at the bottom of the page, like this:

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.



### Strikethrough

~~The world is flat.~~

### Task List (not supported in VS Code)

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

### Emoji (not supported in VS Code)

That is so funny! :joy:

(See also [Copying and Pasting Emoji](https://www.markdownguide.org/extended-syntax/#copying-and-pasting-emoji))


## Extended Syntax NOT Working on github and VS Code


### Highlight

I need to highlight these ==very important words==.

### Subscript

H~2~O

### Superscript

X^2^


### Heading ID

### My Great Heading {#custom-id}

### Definition List
here i dont need to style what is def tile and what is definition it will be rendered as a definition list automatically


term
: definition