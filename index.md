# Headings

There are two ways to create headings:

1. Using `#` followed by a space  
2. Using `=` (equals) and `-` (hyphens) on the next line  

The `=` and `-` method only supports **two heading levels**.  
Always include **blank lines before and after headings** for better compatibility.

## Headings with `#`
# 1  
## 2  
### 3  
#### 4  
##### 5  
###### 6  

## Headings with `=` and `-`
Heading 1  
=  

Heading 2  
-  

# Paragraphs

To create paragraphs, no special symbol is required — just use a **blank line** to separate them.

⚠️ Don’t indent paragraphs with spaces or tabs unless inside a list.

# Line Breaks

To create a line break, use one of these:

| Method                | Status           | Notes                                  |
|----------------------|------------------|----------------------------------------|
| `<br>`               | ✅ Recommended   | Clear and visible                      |
| Two or more spaces   | ✅ Best Practice | Works widely, but hard to see in code  |
| Backslash `\`        | ❌ Not Reliable  | Not widely supported                   |
| Just Enter/Return    | ❌ Not Reliable  | Depends on renderer                    |

# Emphasis

Use `*` or `_` to style text:

- *Italic*: `*text*` or `_text_`  
- **Bold**: `**text**` or `__text__`  
- ***Bold Italic***: `***text***` or `___text___`

⚠️ Prefer `*` over `_` — underscores can break mid-word.

# Blockquotes

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
## Blockquotes with Other Elements

Blockquotes can include other Markdown elements, but **not all will render properly**.  
Test as needed.


# Lists

Use tabs for nested items. and **do not indent** the first item of a list. 
And to add elements like blockquotes or code blocks inside lists, indent them **four spaces** or **one tab**.

## Unordered Lists

Create unordered lists by starting each item with `*`, `-`, or `+` followed by a space. Use one symbol consistently.

## Ordered Lists

Create ordered lists by starting each item with `1.` followed by a space.

| Recommended | Not recommended |
| ----------- | --------------- |
| `1.`        | `1)`            |

If you want a list item starting with a number and period (not list numbering), escape the period with a backslash:

```markdown
- 1968\. A great year!
```

renders as:

* 1968\. A great year!

---

# Code Blocks

Create code blocks using three backticks (\`\`\`).
If your code contains backticks, use double backticks for the fence:

Example:

```markdown
``Use `code` in code block.``
```

---

# Horizontal Rule (HR)

Create a horizontal rule with **3 or more** asterisks (`***`), dashes (`---`), or underscores (`___`) on a line alone.

Add blank lines **before and after** for best compatibility.

Examples:

```
***

---

___
```

---


# Links 

1. **Basic Link**

```markdown
[Link Text](URL)
```

2. **Link with title (tooltip)**

```markdown
[Link Text](URL "Title")
```

3. **Auto-links for URLs or emails**

```markdown
<https://example.com>
<email@example.com>
```

4. **Formatting links**

* Bold: `**[text](URL)**`
* Italic: `*[text](URL)*`
* Code style: ``[`code`](URL)``

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

6. **Best Practices**

* Encode spaces as `%20` in URLs
* Encode parentheses as `%28` and `%29` or use HTML `<a>` tags
* Avoid spaces in URLs directly

Easy version for **Images in Markdown**:

# Images

* To add an image:

```markdown
![Alt text](image-url)
```

* To add a caption, put italic text **below** the image:

```markdown
![Trail](/path/image.jpg)  
*This is the caption.*
```

* To make the image a **link**, wrap the image Markdown in `[ ]` and add the link in `( )`:

```markdown
[![Alt text](image-url "Image title")](link-url)
```

Example:

```markdown
[![Rock](/rock.jpg "Rock photo")](https://example.com)
```

Done.


# Escaping Characters

\* Without the backslash, this would be a bullet in an unordered list.
The rendered output looks like this:

* Without the backslash, this would be a bullet in an unordered list.

Characters You Can Escape
You can use a backslash to escape the following characters.

Character	Name
\	backslash
`	backtick (see also escaping backticks in code)
*	asterisk
_	underscore
{ }	curly braces
[ ]	brackets
< >	angle brackets
( )	parentheses
#	pound sign
+	plus sign
-	minus sign (hyphen)
.	dot
!	exclamation mark
|	pipe (see also escaping pipe in tables)


# HTML
For security reasons, not all Markdown applications support HTML in Markdown documents. When in doubt, check your Markdown application’s documentation. Some applications support only a subset of HTML tags.

Use blank lines to separate block-level HTML elements like <div>, <table>, <pre>, and <p> from the surrounding content. Try not to indent the tags with tabs or spaces — that can interfere with the formatting.

You can’t use Markdown syntax inside block-level HTML tags. For example, <p>italic and **bold**</p> won’t work.