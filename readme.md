
Click here for a complete guide : https://muhammedsuhaib.github.io/.mdOnTheGoo/

# Markdown Cheat Sheet

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

* First item
* Second item
* Third item

### Code

`code`

### Horizontal Rule

---

### Link

[Markdown Guide](https://www.markdownguide.org)

### Image

![alt text](https://www.markdownguide.org/assets/images/tux.png)

### Automatic URL to Link

Just paste the URL and it will be converted to a link automatically:
[http://www.example.com](http://www.example.com)

## ✅ Extended Syntax (Working on GitHub)

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

* [Click here for Tables](docs/markdownGo.md#tables)

### Fenced Code Block (Language-specific code block)

Code blocks with syntax highlighting can be done using either backticks or tildes.
Backticks are more common and recommended.

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

You don’t have to put footnotes at the end of the document. You can put them anywhere except inside other elements like lists, blockquotes, and tables.

### Strikethrough

~~Just need two tildes.~~
VS Code supports it but sometimes behaves oddly.

### Task List (not supported in VS Code)

* [x] Write the press release
* [ ] Update the website
* [ ] Contact the media

### Emoji (not supported in VS Code)

That is so funny! \:joy:


## ❌ Extended Syntax NOT Working on GitHub and VS Code

### Highlight

I need to highlight these ==very important words==.
ALT:
I need to highlight these <mark>very important words</mark>.

### Subscript

H~~2~~O
ALT: H<sub>2</sub>O

### Superscript

X^2^
ALT: X<sup>2</sup>

### Heading ID

### My Great Heading {#custom-id}

You can link to headings with custom IDs in the file by creating a standard link with a number sign (#) followed by the custom heading ID. These are commonly referred to as anchor links.

`[Heading IDs](#custom-id)` [Heading IDs](#custom-id)
Other websites can link to the heading by adding the custom heading ID to the full URL of the webpage (e.g., [Heading IDs](https://www.markdownguide.org/extended-syntax#heading-ids)).

### Definition List

Here I don’t need to style what is a term and what is a definition; it will be rendered as a definition list automatically.

term
: definition

## ⚠ Works but Deprecated

### Center

Markdown has no direct way to center text, but HTML can be used:

```html
<center>This text is centered.</center>
```

<center>This text is centered.</center>

### Color

```html
<font color="red">This text is red!</font>
```

<font color="red">This text is red!</font>

---
