---
layout: default
title: Create a README with Markdown
nav_order: 5
---

# Create a README with Markdown
{: .no_toc }

We will take a look at a README file to demonstrate some common Markdown elements. We will be using this project as a starting point:

>Davis, Matthew, 2024, "Soil Adsorption Curves and Environmental Soil Data", <a href="https://doi.org/10.5683/SP3/JGRIN0" target="_blank">https://doi.org/10.5683/SP3/JGRIN0</a>, Borealis, V1

Take a look at our raw code version of the [README template](https://ubc-library-rc.github.io/rdm/content/exercise_files/README_template.txt) and see if you can make sense of it. Can you make sense of the raw document? What are some things you noticed that are different from a WYSIWYG file?

## Getting started

To get started, you can use a text editor such as [Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown) and create a new file with .md extension to create a Markdown file. Alternatively, if you do not want to download anything, there are several online Markdown editors where you can learn the syntax without downloading anything. Several tools exists. For example, [Dillinger](https://dillinger.io/) and [Markdown Live Preview](https://markdownlivepreview.com/) are great online Markdown editors. You can just open the site and start using Markdown. The text will be on the left pane and the rendered document will be on the right pane.

## Headings

To create a heading, add the number sign (#) in front of your header. The number of number signs will correspond to the header level. 

# This is level 1 (biggest)
## This is level 2
### This is level 3
#### This is level 4
##### This is level 5
###### This is level 6

When you use a header, always put a space between the number sign and the start of your header
* `# Add a space after your header`
* `#No space after header`

Also, you should add new lines before and after the header.

## Paragraph and line breaks

To create paragraphs, use a new line. Further, to force a new line, you can add a `\` or `<br>` at the end of the line.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## **Bold** and *Italic*

You can bold a word/phrase by wrapping it around a double asterisks or double underscore.

* **Asterisks to bold** `**Asterisks to bold**`
* __Underscore to bold__  `__Underscore to bold__`

You can italicize a word/phrase by wrapping it around a single asterisks or single underscore.

* *Asterisks to italicized* `*Asterisks to italicized*`
* _Underscore to italicized_  `_Underscore to italicized_`

## Bold and italic together

You can bold and italic together wrapping the word/phrase around three asterisks or three underscores.

* ***This is something really important*** `***This is something really important***`
* ___This is something really important___ `___This is something really important___`

# Unordered lists

To create an unordered list, you need an asterisk (*), dash (-), or a plus sign (+) in front of the item. For nested unordered lists, indent the items you want indented.

| **Markdown code**                          | **What you see**                                     |
|--------------------------------------------|------------------------------------------------------|
| `* Item`<br>`* Item`                       | <ul> <li>Item <li>Item </ul>                         |
| `- Also an item`<br>`- Also an item`       | <ul> <li>Also an item <li>Also an item </ul>         |
| `+ This also works`<br>`+ This also works` | <ul> <li> This also works <li> This also works </ul> |
| `* This is level one`<br>`* This is level one`<br> | <ul> <li> This is level one <li> This is level one </ul> |
| `* This is level one`<br>`* This is level one`<br>`  * This is level two` | <ul> <li> This is level one <li> This is level one <ul> <li> This is level two </ul> </ul> |

# Ordered lists

To create an ordered list, add numbers followed by a period (1.) Again, for nested ordered list, indent the items you want indented. Note that the numbers do not have to be in order, but they should start with 1.

| **Markdown code**                                      | **What you see**                                                  |
|--------------------------------------------------------|-------------------------------------------------------------------|
| `1. Item`<br>`2. Item`                                 | <ol> <li>Item</li> <li>Item</li> </ol>                           |
| `1. First item`<br>`1. Second item`                     | <ol> <li>First item</li> <li>Second item</li> </ol>               |
| `1. This works too`<br>`9. Another item`                | <ol> <li>This works too</li> <li>Another item</li> </ol>          |
| `1. Level one`<br>`2. Level one`<br>`  1. Level two`   | <ol> <li>Level one</li> <li>Level one <ol> <li>Level two</li> </ol> </li> </ol> |

## Unordered list with ordered list

You can nest an ordered list in an unordered list and vice versa.

1. Item 1
2. Item 2
    * No order item 1
    * No order item 2
3. Item 3

* Item 1 
* Item 2
    1. Ordered item 1
    2. Ordered item 2
* Item 3

# Link 

Adding links is something that is very common. To create a link, wrap the link text in square brackets [Google] and the url link immediately after in parentheses (https://www.google.com/).

This is what the Markdown syntax looks like:

`You can find more workshops from UBC RDM from our [online textbook](https://ubc-library-rc.github.io/rdm/)!`

This will render to something that looks like this:

You can find more workshops from UBC RDM from our [online textbook](https://ubc-library-rc.github.io/rdm/)!

# Images

To add images in your Markdown file, the syntax is similar to adding a link for an url. Add the alternative text for screen readers in the square brackets `![]` followed by the path to the image in parenthesis `()`.

This is what the Markdown syntax looks like:

`![](images/bottles.jpg)`

This will render to something that looks like this:

<img src="images/bottles.jpg" width="300" height="200">

# Exercise 
{: .no_toc}

Let's take a look at the [README template](https://ubc-library-rc.github.io/rdm/content/exercise_files/README_template.txt) again. Does this document make more sense now? Can you think of some ways that we can improve the README file?

# Congrats!
{: .no_toc }

You now know how to use Markdown and should be able to use it for creating documents. Join us next time for some more advanced Markdown syntax.

### Sources
{: .no_toc }
- Markdown Guide. <https://www.markdownguide.org/>
- Basic writing and formatting. <https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax>
- The Ultimate Guide to Markdown. <https://gist.github.com/cuonggt/9b7d08a597b167299f0d>
- Handbook Markdown Guide. <https://handbook.gitlab.com/docs/markdown-guide/>

---

Need help?
{: .label .label-blue }
  Please reach out to `research.data@ubc.ca` for assistance with any of your research data questions.
