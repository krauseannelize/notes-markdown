# Guide to Markdown

As someone who has spent two decades editing and formatting legal documents, Markdown was the logical starting point when I started to learn code and using Git. Its simplicity, readability, and versatility make it an ideal tool for writing and maintaining documentation.

This guide aims to provide a concise overview of Markdown syntax and best practices. It's primarily intended as a quick reference for myself, but I hope it will also be helpful to others who are new to Markdown or looking to refresh their knowledge.

## Contents
1. [Paragraphs](#paragraphs)
2. [Emphasis](#emphasis)
3. [Headings](#headings)
4. [Horizontal Line](#horizontal-line)
5. [Links](#links)
	- [Create a link](#links-create)
	- [Reference links](#links-reference)
	- [Add tooltips](#links-tools)
	- [Convert URLs or email addresses to links](#links-email)
6. [Images](#images)
7. [Lists](#lists)
	- [Ordered lists](#lists-ordered)
	- [Unordered lists](#lists-unordered)
	- [Nested lists](#lists-nested)
	- [Task lists](#lists-task)
8. [Blockquote](#blockquote)
9. [Tables](#tables)
	- [Creating tables](#tables-create)
	- [Table alignment](#tables-align)
	- [Formatting text inside tables](#tables-format)
10. [Cross-Referencing](#cross-referencing)

---

<a name="paragraphs" />

### Paragraphs

Create paragraphs by entering text without any symbols. Remember to use a blank line to separate one or more lines of text.

##### Input:

```
Text line 1

Text line 2
```

##### Output:

Text line 1

Text line 2

---

<a name="emphasis" />

### Emphasis

Text can be emphasized by encapsulating words or phrases in a combination of symbols.

| Style | Input | Output |
| :-- | :-- | :-- |
| Italics | `*1 asterisk* or _1 underscore_` | *1 asterisk* or _1 underscore_ |
| Bold | `**2 asterisks** or __2 underscores__` | **2 asterisks** or __2 underscores__ |
| Bold and italics | `***3 asterisks***` | ***3 asterisks*** |
| Bold and nested italics | `**2 symbols and _1 to nest_**` | **2 symbols and _1 to nest_** |
| Italics and nested bold | `*1 symbol and __2 to nest__*` | *1 symbol and __2 to nest__* |
| Strike-through | `~~2 tildes~~` | ~~2 tildes~~ |
| Subscript | `<sub>Sub tag</sub> for subscript` | <sub>Sub tag</sub> for subscript |
| Superscript | `<sup>Sup tag</sup> for superscript` | <sup>Sup tag</sup> for superscript |

---

<a name="headings" />

### Headings

To create a heading, add the hash symbol (#) in front of the heading text. The number of
hash symbols correspond to the heading level and you can have up to 6 heading levels. Remember to add a space between the hash symbol and the text for ensure compatibility.

##### Input: 

```
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6
```

##### Output:

# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6

---

<a name="horizontal-line" />

### Horizontal line

Horizontal lines are used to visually separate sections within a document to provide a clear break. Insert a horizontal line by putting three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

##### Input:

```
Line with asterisks

***

Line with dashes

---

Line with underscores

___

```

##### Output:

Line with asterisks

***

Line with dashes

---

Line with underscores

___

It is best practice to add a blank line before and after a horizontal line for compatibility.

---

<a name="links" />

### Links

<a name="links-create" />

#### Create a link

GitHub automatically create a clickable link when a valid URL is entered displaying the entire URL. However, if you would like to display text instead of the URL, you can do so by enclosing the text you would like to be displayed in square brackets ( [ ] ) followed by the URL in round brackets ( ( ) ).

##### Input:

```
https://github.com/krauseannelize
[My Github page](hhttps://github.com/krauseannelize)
```

##### Output:

https://github.com/krauseannelize
[My Github page](hhttps://github.com/krauseannelize)

<a name="links-reference" />

#### Reference links

When you need to refer to the same URL multiple times, you can use reference links to create links that refer to specific definitions. You can do this by placing the definition in square brackets ( [ ] ), followed by a colon (:), a space and then the URL as is or enclosing it in left and right angle brackets ( < > ). Refer to the reference link by inserting the text you would like to display in square brackets ( [ ] ) followed by round brackets ( ( ) ) containing the definition.

##### Input:

```
[my-github]: https://github.com/krauseannelize

See what I've been up to on Github [here](mygithub).
Using the same definition [again](my-github).
```

##### Output:

[my-github]: https://github.com/krauseannelize

See what I've been up to on Github [here](mygithub).
Using the same definition [again](my-github).

<a name="links-tools" />

#### Add tooltips

You can display a handy tooltip when someone hovers over the link with a mouse by adding the tooltip you would like to display in quotation marks ( " " ) following the URL in the round brackets ( ( ) ).

##### Input:

```
[My Github page](hhttps://github.com/krauseannelize "See what I've been up to!")
```

##### Output:

[My Github page](hhttps://github.com/krauseannelize "See what I've been up to!")

<a name="links-email" />

#### Convert URLs or email addresses to links

You can turn a URL or email address into a clickable link by enclosing it in left and right angle brackets ( < > ).

##### Input:

```
<email@example.com>
```

##### Output:

<email@example.com>

---

<a name="images" />

### Images

To add an image, add an exclamation mark (!), followed by alt text in square brackets ( [ ] ) and the path or URL to the image in round brackets ( ( ) ). in parentheses. An optional title that will be displayed when you hover over the image with a mouse can be added by inserting the text in quotation marks ( " " ) following the URL in the round brackets ( ( ) ).

Always provide descriptive alt text within the square brackets for accessibility. This text will be displayed if the image cannot be loaded.

##### Input:

```
Image stored in repository's root directory:
![The Markdown Logo](Markdown-Logo.png "The Markdown Logo")

Image stored in a subdirectory of the repository:
![The Markdown Logo](images/Markdown-Logo.png "The Markdown Logo")

Image inserted from a URL:
![The Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/175px-Markdown-mark.svg.png "The Markdown Logo")
```

##### Output:


Image stored in repository's root directory:
![The Markdown Logo](Markdown-Logo.png "The Markdown Logo")

Image stored in a subdirectory of the repository:
![The Markdown Logo](images/Markdown-Logo.png "The Markdown Logo")

Image inserted from a URL:
![The Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/175px-Markdown-mark.svg.png "The Markdown Logo")

---

<a name="lists" />

### Lists

Markdown allows you to create both ordered and unordered lists, which can be combined to create nested lists. Additionally, you can create a list with checkboxes that can be checked or unchecked to keep track of tasks.

<a name="lists-ordered" />

#### Ordered lists

Create an ordered list by starting each new line item with a number followed by a period. As long as you start with 1, the rest of the list _does not have to be entered in numerical order_. For compatibility, only use periods and do not use brackets.

##### Input:

```
Numbers in numerical order:
1. Line item 1
2. Line item 2
3. Line item 3

Numbers not in numerical order:
1. Line item 1
9. Line item 2
4. Line item 3

Using just number 1:
1. Line item 1
1. Line item 2
1. Line item 3
```

##### Output:

Numbers in numerical order:
1. Line item 1
2. Line item 2
3. Line item 3

Numbers not in numerical order:
1. Line item 1
9. Line item 2
4. Line item 3

Using just number 1:
1. Line item 1
1. Line item 2
1. Line item 3

<a name="lists-unordered" />

#### Unordered lists

Create an unordered list of items without a specific order or numbering system by starting each new line item with either an asterisk (*), a dash (-), or a plus sign (+). For compatibility, do not mix and match symbols in the same list and use one symbol per list.

If you need to start an unordered list item with a number followed by a period, you can use a backslash (\\) before the number to escape the formatting.

##### Input:

```
List with asterisks:
* Line item 1
* Line item 2
* Line item 3

List with dashes:
- Line item 1
- Line item 2
- Line item 3

List with plus signs:
+ Line item 1
+ Line item 2
+ Line item 3
```

##### Output:

List with asterisks:
* Line item 1
* Line item 2
* Line item 3

List with dashes:
- Line item 1
- Line item 2
- Line item 3

List with plus signs:
+ Line item 1
+ Line item 2
+ Line item 3

<a name="lists-nested" />

#### Nested lists

You can combine both ordered and unordered lists to create nested lists by indenting one or more line items with four spaces or one tab. You cannot create a numbered nested list with indentation. Indentation will change the bullet character up to 3 times and you do not have to mix and match symbols. It is best practice not to indent more than 2 times.

##### Input:

```
1. Numbered line item 1
* Bulleted line item
* Bulleted line item
	* Nested bulleted line item
		* Sub-nested bulleted line item
2. Numbered line item 3
3. Numbered line item 4
```

##### Output:

1. Numbered line item 1
* Bulleted line item
* Bulleted line item
	* Nested bulleted line item
		* Sub-nested bulleted line item
2. Numbered line item 3
3. Numbered line item 4

<a name="lists-task" />

#### Task lists

Keep track of tasks with checked or unchecked boxes by creating a task list. Add a dash (-) followed by  square brackets containing a space ([ ]) to the beginning of the task list item. This will create an unchecked box. To create a checked box, replace the space in the square brackets with an x ([x]).

##### Input:

```
- [ ] Task item 1
- [x] Task item 2
- [ ] Task item 3
```

##### Output:

- [ ] Task item 1
- [x] Task item 2
- [ ] Task item 3

---

<a name="blockquote" />

### Blockquote

Blockquote is used when you need to highlight important text, cite a source, quote someone or create a dialogue. Create a blockquote by starting a paragraph with a right angle bracket (>). A blockquote can contain multiple paragraphs by starting each paragraph and blank line between the paragraphs with a right angle bracket. Nested blockquotes can be created by using multiple right angle brackets to indent. It is best practice to add a blank line before and after blockquotes for compatibility.

##### Input:

```
What a regular paragraph looks like
> compared to a block quote paragraph.

A block quote with
> multiple paragraphs looks
> 
> like this.

Create a dialogue
> by quoting someone
>> that quoted someone else
>>> using nested paragraphs.
```

##### Output:

What a regular paragraph looks like
> compared to a block quote paragraph.

A block quote can have
> multiple paragraphs by simply
> 
> using a right angle bracket in front of a blank line.

Create a dialogue
> by quoting someone
>> that quoted someone else
>>> using nested paragraphs.
>
---

<a name="tables" />

### Tables

Information can be displayed in a neat and organized fashion by arranging it in rows and columns to create a table.

<a name="tables-create" />

#### Creating tables

Start and end every row with a pipe (|) for compatibility and use a pipe to separate each column. To create a column header, use three or more dashes (---). For a table to render correctly, you must include a blank line before the table and include a header row. You can add additional spaces to align the input for readability, but the rendered output will look the same without it.

##### Input:

```
Table with additional spaces:
| Header 1 | Header 2 | Header 3 |
| ---      | ---      | ---      |
| Item 1   | Item 2   | Item 3   |

Table without additional spaces:
| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Item 1 | Item 2 | Item 3 |
```

##### Output:

Table with additional spaces:
| Header 1 | Header 2 | Header 3 |
| ---      | ---      | ---      |
| Item 1   | Item 2   | Item 3   |

Table without additional spaces:
| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Item 1 | Item 2 | Item 3 |

<a name="tables-align" />

#### Table alignment

By default, the table will align all text in the table to the left. You can change the alignment in the row that creates the header with three or more dashes (---) by adding a colon (:) to the:

- left for left alignment ( :--- )
- right for right alignment ( ---: )
- left and right for center alignment ( :---:)

##### Input:

```
| Left | Center | Right |
| :--- | :---: | ---: |
| alignment | alignment | alignment |
| item | item | item |
```

##### Output:

| Left | Center | Right |
| :--- | :---: | ---: |
| alignment | alignment | alignment |
| item | item | item |

<a name="tables-format" />

#### Formatting text inside tables

Formatting that you can use inside tables:

- [Paragraphs](#paragraphs)
- [Emphasis](#emphasis)
- [Links](#links)
- {code with backticks}

Formatting that you cannot use inside tables:

- [Headings](#headings)
- [Horizontal line](#horizontal-line)
- [Images](#images)
- [Lists](#lists)
- [Blockquotes](#blockquotes)- 
- {code blocks, or HTML tags}

---

<a name="cross-referencing" />

### Cross-referencing

Reference to another part of the document by inserting an anchor point and inserting a link to that anchor point. It is useful to place the anchor point right before the section in the document it is referring to.

##### Input:

```
Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

#### Anchor Point
```

##### Output:

Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

#### Anchor Point

---