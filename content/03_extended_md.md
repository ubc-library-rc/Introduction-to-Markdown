---
layout: default
title: Advanced Markdown
nav_order: 6
---

# Advanced Markdown 

In the previous workshops, we outlined what it is and the basic syntax to get started. This workshop will show you more advanced syntax and some workarounds for the limitations of Markdown.

# Tables 

Tables in Markdown are created with at least three hyphens `(---)` to create the column header and pipes `(|)` to separate the columns. This is how you create a table in Markdown:

```
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Stuff    | Markdown | Table    |
| Stuff    | Markdown | Table    |
```

This will render to the following:

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Stuff    | Markdown | Table    |
| Stuff    | Markdown | Table    |

However, making tables in Markdown by hand is difficult and tedious. We suggest using a Markdown table generator instead. Here are some tools you can use:

* [Tables Generator](https://www.tablesgenerator.com/markdown_tables)
* [TableConvert](https://tableconvert.com/markdown-generator)
* [Table to Markdown](https://tabletomarkdown.com/generate-markdown-table/)

### Emphasizing in tables 

You can use bold, italics, urls and code in tables. The syntax is the same.

| Column 1  | Column 2       | Column 3 |
|-----------|----------------|----------|
| **Stuff** | **_Markdown_** | `Table`  |
| _Stuff_   | **_Markdown_** | [Table]()|

### Alignment in tables

You can add alignment in tables by adding a colon `(:)` to the left, right, or both side of the hyphens within the header row.

```
| Column 1 | Column 2 | Column 3 |
|----------|:--------:|---------:|
| Left     | Center   | Right    |
| Left     | Center   | Right    |
```

This will generate to:

| Column 1 | Column 2 | Column 3 |
|----------|:--------:|---------:|
| Left     | Center   | Right    |
| Left     | Center   | Right    |

# Using HTML in Markdown 

You can already do many things with the content from the basics and advanced Markdown workshops, but there are some things that Markdown does not support. Many of these limitations can be "solved" with HTML. Here we will go over some useful "solutions" for common tools needed for a paper or report.

## Lists in a table

You cannot add a list in a table in Markdown, if you need to, you can use HTML.

```
<ol>
    <li>Level one</li>
    <li>Level one
        <ol>
            <li>Level two</li>
        </ol>
    </li>
</ol>

```

| **Markdown code**                                      | **What you see**                                                                |
|--------------------------------------------------------|---------------------------------------------------------------------------------|
| `1. Level one`<br>`2. Level one`<br>`  1. Level two`   | <ol> <li>Level one</li> <li>Level one <ol> <li>Level two</li> </ol> </li> </ol> |

## Line breaks in a table 

You can add a new line in a table if you use the `<br>` tag. 

```
| One line | Two line                       |
|----------|--------------------------------|
| Item 1   | Item 1 <br> Item 2 <br> Item 3 |
```

This will render to this table:

| One line | Two line                       |
|----------|--------------------------------|
| Item 1   | Item 1 <br> Item 2 <br> Item 3 |

## Underline

If you want to underline a word or phrase, you can use the `<u>` HTML tag. The following will produce and underline:

`<u>This sentence is underlined</u>`

This it will look like this:

<u>This sentence is underlined</u>

## Font color

The `<font>` HTML tag will allow you to change the font color of your text in Markdown.

```
<font color="blue"> This sentence is blue.</font> <font color="green">And this sentence is green.</font><font color="red"> Lastly, this sentence is red.</font>
```

This is what it returns:

<font color="blue"> This sentence is blue.</font> <font color="green">And this sentence is green.</font><font color="red"> Lastly, this sentence is red.</font>

# Comments

Comments are often used when writing WYSIWYG documents and in programming. The comment-out used in HTML can be used in Markdown as well. To comment out something in Markdown (and HTML), wrap the text or phrase in `<!--Text-->`. Anything wrapped in the double dash will not show up in the rendered product.

# Image Size

The syntax for images in Markdown is simple but does not allow for sizing. You can use the `<img>` HTML tag, and you can change the `width` and `height` attributes to adjust the size.

`<img src="images/bottles.jpg" width="200" height="100">`

This controls the size: 

<img src="images/bottles.jpg" width="200" height="100">

# Congrats!
{: .no_toc }

You have learned some advanced Markdown hacks and workarounds using HTML for common tools in WYSIWYG documents.

### Sources
{: .no_toc }
- Markdown Guide. <https://www.markdownguide.org/>
- Basic writing and formatting. <https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax>
- Handbook Markdown Guide. <https://handbook.gitlab.com/docs/markdown-guide/>
- The Ultimate Guide to Markdown. <https://gist.github.com/cuonggt/9b7d08a597b167299f0d>

---

Need help?
{: .label .label-blue }
  Please reach out to `research.data@ubc.ca` for assistance with any of your research data questions.
