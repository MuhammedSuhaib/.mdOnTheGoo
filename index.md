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
>>>>>>>>>>>>>>> Most renderers support 10–15 levels  
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> 100



>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> VSCode can handle 101+

## Blockquotes with Other Elements

Blockquotes can include other Markdown elements, but **not all will render properly**.  
Test as needed.
