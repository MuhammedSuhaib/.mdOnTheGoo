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
use tabs for nested items

Adding Elements in Lists
To add another element like a blockquote or code block etc, indent the element four spaces or one tab.

## Unordered Lists
To create an unordered list, start each item with `*`, `-`, or `+` followed by a space. use any one of these symbols consistently.

## Ordered Lists
To create an ordered list, start each item with `1.` followed by a space.

| 1. | 1)|
| recommended | not recommended|

If you need to start an unordered list item with a number followed by a period, you can use a backslash (\) to escape the period.
`- 1968\. A great year!` => `- 1968. A great year!`


# code blocks
To create a code block, use three backticks (` `) or if there is an exitsing bacticked element in that block so use double backtick


like:
``Use `code` in code block.``


# hr
To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.For compatibility, put blank lines before and after horizontal rules.



1. ***

2. ---

3. ___


# Links
To create a link, use the `[]` for hypertext and `()` for the URL.
like: `[Link Text](https://example.com)` this will look like [Link Text](https://example.com)