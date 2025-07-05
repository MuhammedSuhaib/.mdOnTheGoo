
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

* [Click here for Tables](docs/index.md#tables)

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

I need to highlight these ==very important words==.   (Not Working ❌)

**Alternately You can use :**   

I need to highlight these <mark>very important words</mark>. (Working ✅)

### Subscript

H~~2~~O   (Not Working ❌)

**Alternatively You can use :**    

H<sub>2</sub>O (Working ✅)

### Superscript

X^2^   (Not Working ❌)

**Alternatively You can use :**    

X<sup>2</sup> (Working ✅)

### Heading ID

### My Great Heading {#custom-id}

You can link to headings with custom IDs in the file by creating a standard link with a number sign (#) followed by the custom heading ID. These are commonly referred to as anchor links.

`[Heading IDs](#custom-id)` [Heading IDs](#custom-id)
Other websites can link to the heading by adding the custom heading ID to the full URL of the webpage (e.g., [Heading IDs](https://www.markdownguide.org/extended-syntax#heading-ids)).

### Definition List

Here I don’t need to style what is a term and what is a definition; it will be rendered as a definition list automatically.

term  
: definition

## ⚠ Works on Vscode but (not supported on Github)

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
## jekyll-theme

To add a jekyll theme , you can add the following line to your `_config.yml` file:

```yaml
theme: jekyll-theme-theme-name
```

this will apply the specified theme to your Jekyll site. Make sure to replace `theme-name` with the actual name of the theme you want to use.

Available themes can be found at [Jekyll Themes](https://pages.github.com/themes/).
Jekyll themes only affect deployed sites, not the normal `.md` files in a repo.
normal `.md` files use GitHub’s default markdown renderer, not Jekyll.
