# Basic Syntax

## Headings

There are two ways to create headings:

1. Using `#` followed by a space  
2. Using `=` (equals) and `-` (hyphens) on the next line  

The `=` and `-` method only supports **two heading levels**.  
Always include **blank lines before and after headings** for better compatibility.

### Headings with `#`
# 1  
## 2  
### 3  
#### 4  
##### 5  
###### 6  

### Headings with `=` and `-`
Heading 1  
=  

Heading 2  
-  


## Paragraphs

To create paragraphs, no special symbol is required — just use a **blank line** to separate them.

⚠️ Don’t indent paragraphs with spaces or tabs unless inside a list.

## Line Breaks

To create a line break, use one of these:

| Method                | Status           | Notes                                  |
|----------------------|------------------|----------------------------------------|
| `<br>`               | ✅ Recommended   | Clear and visible                      |
| Two or more spaces   | ✅ Best Practice | Works widely, but hard to see in code  |
| Backslash `\`        | ❌ Not Reliable  | Not widely supported                   |
| Just Enter/Return    | ❌ Not Reliable  | Depends on renderer                    |


## Spaces

Use `&nbsp;` to add a single space between words or elements.

Or 

You can use `<pre>` to display all spaces & blanks you have typed. E.g.:

<pre>
Hi,   I  am  using             a lot
   of  spaces     here   

      ....
</pre>

---

## Horizontal Rule (HR)

Create a horizontal rule with **3 or more** asterisks (`***`), dashes (`---`), or underscores (`___`) on a line alone.

Add blank lines **before and after** for best compatibility.

Examples:

```
***

---

___
```

---

## Emphasis

Use `*` or `_` to style text:

- *Italic*: `*text*` or `_text_`  
- **Bold**: `**text**` or `__text__`  
- ***Bold Italic***: `***text***` or `___text___`
- <u>Underlined</u>: text is not supported. But you can use HTML `<u>` tag: `<u>text</u>`
- ~~Strikethrough~~: `~~text~~`  
⚠️ Prefer `*` over `_` — underscores can break mid-word.


## Lists

Use tabs for nested items. and **do not indent** the first item of a list. 
And to add elements like blockquotes or code blocks inside lists, indent them **four spaces** or **one tab**.

### Unordered Lists

Create unordered lists by starting each item with `*`, `-`, or `+` followed by a space. Use one symbol consistently.

### Ordered Lists

Create ordered lists by starting each item with `1.` followed by a space.

| Recommended | Not recommended |
| ----------- | --------------- |
| `1.`        | `1)`            |

If you want a list item starting with a number and period (not list numbering), escape the period with a backslash:

```markdown
- 1968\. A great year!
```

Renders as:

⇒ 1968\. A great year!

---

## Links 

1. **Basic Link**

```markdown
[Link Text](URL)
```
Renders as:


⇒ [Link Text](URL)


2. **Link with title (tooltip)**

```markdown
[Link Text](URL "Title")
```

Renders as:


⇒ You will see a tooltip when you hover over the link below.  
⇒ [Link Text](URL "Title") 

3. **Auto-links for URLs or emails**

```markdown
<https://example.com>
<email@example.com>
```

Renders as:

⇒ <https://example.com>   
⇒ <email@example.com>


4. **Formatting links**

* Bold: `**[text](URL)**`
* Italic: `*[text](URL)*`
* Code style: ``[`code`](URL)``

Renders as:

⇒  Bold: **[text](URL)**  
⇒  Italic: *[text](URL)*  
⇒  Code style: ``[`<code>`](URL)``


5. **Reference-style links** (split in two parts)

* Inline: `[text][label]` or `[text] [label]` (can work with a space or without a space both work)
* Definition (anywhere in file):

  ```markdown
  [label]: URL "Optional title"
  ```
* Example:

  ```markdown
  [hobbit-hole][1] when i click this it will take me where the 1 is defined
  ...
  [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
  ```

Renders as:

⇒ [hobbit-hole][1] when i click this it will take me where the 1 is defined   
  ...   
⇒ [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles" 

6. **Best Practices**

* Encode spaces as `%20` in URLs
* Encode parentheses as `%28` and `%29` or use HTML `<a>` tags
* Avoid spaces in URLs directly


## Images

* To add an image:

```markdown
![Alt text](image-url)
```

* To add a caption, put italic text **below** the image:

```markdown
![Trail](/path/image.jpg)  
*This is the caption.*
```
For example:

⇒ ⇢⇢ ⇢⇢  ⇢⇢  ⇢⇢  ⇢⇢   ![Mind-Blowing Experiment](https://img.youtube.com/vi/kn1oT-VGxhI/0.jpg)  
⇒ ⇢⇢ ⇢⇢  ⇢⇢  ⇢⇢  ⇢⇢   *How 1 Pixel Actually Looks Like!*


* To make the image a **link**, wrap the image Markdown in `[ ]` and add the link in `( )`:

```markdown
[![Alt text](image-url "Image title")](link-url)
```

Example:

```markdown
[![Rock](/rock.jpg "Rock photo")](https://example.com)
```

Done.

## Video

For embedding videos, you can use the following Markdown syntax. Replace `YOUTUBE-ID` with the actual ID of the YouTube video you want to embed.
`[![Image alt text](https://img.youtube.com/vi/YOUTUBE-ID/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE-ID)`

[!["This Is What 1 Pixel Actually Looks Like! (Mind-Blowing Experiment)"](https://img.youtube.com/vi/kn1oT-VGxhI/0.jpg)](https://youtu.be/kn1oT-VGxhI)

## Tables

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

Renders as:

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

You can add a list inside a table cell by using HTML tags, because directly adding list elements (`*`, `-`, `+`) won't work. Same for `<br>` tags.

### Table of Contents

```md
- [Horizontal Rule](#horizontal-rule-hr)  
- [Images](#images)  
- [Links](#links)
```

* [Horizontal Rule](#horizontal-rule-hr)
* [Images](#images)
* [Links](#links)



## Blockquotes

To create a blockquote, add `>` before a paragraph.  
Include blank lines **before and after** for compatibility.

> 1 blockquote  
>> 2 blockquote  
>>> 3 blockquote  
>>>> 4 blockquote  
>>>>> 5 blockquote  
>>>>>> 6 blockquote  
>>>>>>> 7 blockquote  
>>>>>>>> 8 blockquote  
>>>>>>>>> 9 blockquote  
>>>>>>>>>> 10 blockquote  
>>>>>>>>>>> 11 blockquote  
>>>>>>>>>>>> 12 blockquote  
>>>>>>>>>>>>> 13 blockquote  
>>>>>>>>>>>>>> 14 blockquote  
>>>>>>>>>>>>>>> Most renderers support 10–15 levels  but vscode supports 100 levels.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> 100🤯
### Blockquotes with Other Elements

Blockquotes can include other Markdown elements, but **not all will render properly**.  
Test as needed.

## Comments

```markdown
Here's a paragraph that will be visible.

[This is a comment that will be hidden.]: # 

And here's another paragraph that's visible.
```

Renders as:

Here's a paragraph that will be visible.

[This is a comment that will be hidden.]: # 

And here's another paragraph that's visible.

## Symbols
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

## Code Blocks

Create code blocks using three backticks (\`\`\`).
If your code contains backticks, use double backticks for the fence:

Example:

```markdown
``Use `code` in code block.``
```
Renders as:

⇒   ``Use `<code>` in code block.``

## Escaping Characters

```
* Without the backslash, this would be a bullet in an unordered list.
```
↴
* Without the backslash, this would be a bullet in an unordered list.   
↴  
\* Without the backslash, this would be a bullet in an unordered list.
The rendered output looks like this:

```
\* Without the backslash, this would be a bullet in an unordered list.
The rendered output looks like this:
```

Characters You Can Escape
You can use a backslash to escape the following characters.
```
Character	Name

\	backslash
`	backtick 
*	asterisk
_	underscore
{ }	curly braces
[ ]	brackets
< >	angle brackets
( )	parentheses
#	hash sign
+	plus sign
-	minus sign (hyphen)
.	dot
!	exclamation mark
|	pipe 

```
## HTML
For security reasons, not all Markdown applications support HTML in Markdown documents. When in doubt, check your Markdown application’s documentation. Some applications support only a subset of HTML tags.

Use blank lines to separate block-level HTML elements like `<div>`, `<table>`, `<pre>`, and `<p>` from the surrounding content. Try not to indent the tags with tabs or spaces — that can interfere with the formatting.

You can’t use Markdown syntax inside block-level HTML tags. For example,
`*italic* and **bold**` won’t work. in html

```html
<p>*italic* and **bold** As you can see it is not working</p>
```