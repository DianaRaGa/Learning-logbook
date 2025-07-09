**Date:** 09 July 2025

# Headings
Using the `#` symbol to create titles and section headings. It makes them bolder and gives them consistent sizes:

`# Big title for headers  `

`## Section inside the title  `

`### Subsection `

***Example:***
# Big title for headers  
## Section inside the title  
### Subsection

---

# Numbered Lists
To create numbered lists in Markdown, simply write it like this:

1. First  
2. Second  
3. Third  

Really helpful for making lists and breaking down a text.

*Note:*  
It can be done with any number, and when rendered, it looks as it should (with the appropriate numbers). How cool!

---

# Bullet Lists
Use `-` at the beginning of the sentence to make a list with bullet points:

- One  
- Two  
    - Two.1

---

# Formatting Text
Using asterisks makes it easy to format text:

## One Asterisk
To make text *italic*, wrap the word in a single asterisk (`*`) — `*like this*`

## Two Asterisks
To make text **bold**, wrap it in double asterisks (`**`) — `**like so**`

## Three Asterisks
To make text ***bold and italic***, use triple asterisks (`***`) — `***like this!***`

# Manual Table of Contents in Markdown (but clickable)
You can make a basic TOC like this:
## 📚 Table of Contents
`- [Introduction](#Title of the section)`

`- [Exercise 1](#exercise-1)`

`- [Exercise 2](#exercise-2)`

`- [Reflection](#reflection)`

🔗 Clicking on any of those links will jump to the matching section in the .md file:  on GitHub, Phoenix Code, 
- Jupyter notebooks, etc.

---

# 🖼️ Markdown Cheat Sheet: Images from Repo Folders
## Basic Image Syntax
Always put this syntax of the image as described below, without the space between the `]` and 
the `(`. It will show the image in the render.

***Example***

`![Alt text](path/to/image.png)`

## 🧠 If .md is in a subfolder (like /chapters/)
Simply use the "`../`" to go up one level as needed.

***Example***

`![Diagram](../images/diagram.png)`

---

# 📋 Markdown Cheat Sheet: Tables

## ✅ Basic Table
The syntax to make a simple table

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1A   | Row 1B   | Row 1C   |
| Row 2A   | Row 2B   | Row 2C   |

## Center / Left / Right Alignment
To make alignment inside the columns

| Left Aligned | Centered | Right Aligned |
|:-------------|:--------:|--------------:|
| Apple        |    🍎    |           Red |
| Banana       |    🍌    |        Yellow |

## ❌ Table Centering (whole table)
- Markdown **cannot center a full table**
- Using HTML trick `<p align="center">`  *may not work in all editors or in a table

---

# 🎨 Markdown Cheat Sheet: Colors

## ❌ Native Markdown doesn't support colors.
It can be a workaround in two ways:

### Use inline HTML (works on GitHub, not all previews)
Using this like of code in HTML for different colors

`<span style="color: red">This text is red</span>`

*Example:*
<span style="color: red">This text is red</span>

### Emoji as visual color cues
🟢 Success  
🔴 Error  
🟡 Warning  
📘 Info  

---

# Showing code examples in Markdown without executing them

1. Use Backticks ` for Inline Code
2. Use Triple Backticks ``` for Code Blocks

## 🔁 Want to specify the language (for highlighting)?
You can also specify the language right after the opening backticks:

```html <p align="center"> Hello!</p> ```

That highlights the code with color (in editors like Phoenix Code, VS Code, etc.)
