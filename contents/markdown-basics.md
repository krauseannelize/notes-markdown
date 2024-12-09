# Markdown Basics

1. [Paragraphs](#paragraphs)
1. [Emphasis](#emphasis)
1. [Headings](#headings)
1. [Horizontal Line](#horizontal-line)
1. [Links](#links)
   - [Create a link](#create-a-link)
   - [Reference links](#reference-links)
   - [Add tooltips](#add-tooltips)
   - [Convert URLs or email addresses to links](#convert-urls-or-email-addresses-to-links)
1. [Images](#images)
1. [Lists](#lists)
   - [Ordered lists](#ordered-lists)
   - [Unordered lists](#unordered-lists)
   - [Nested lists](#nested-lists)
   - [Task lists](#task-lists)
1. [Blockquotes](#blockquotes)
1. [Tables](#tables)
   - [Creating tables](#creating-tables)
   - [Table alignment](#table-alignment)
   - [Formatting text inside tables](#formatting-text-inside-tables)
1. [Cross-referencing](#cross-referencing)
   - [Referencing document sections](#referencing-document-sections)

---

## Paragraphs

Create paragraphs by entering text without any symbols. Remember to use a blank line to separate one or more lines of text.

***Syntax***

```markdown
Text line 1

Text line 2
```

---

***Rendered Output***

Text line 1

Text line 2

---

[back to top](#markdown-basics)

---

## Emphasis

Text can be emphasized by encapsulating words or phrases in a combination of symbols.

| Style | Syntax | Rendered Output |
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

[back to top](#markdown-basics)

---

## Headings

To create a heading, add the hash symbol (#) in front of the heading text. The number of hash symbols correspond to the heading level and you can have up to 6 heading levels. Remember to add a space between the hash symbol and the text for ensure compatibility.

***Syntax***

```markdown
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6
```

---

***Rendered Output***

# Heading level 1

## Heading level 2

### Heading level 3

#### Heading level 4

##### Heading level 5

###### Heading level 6

---

[back to top](#markdown-basics)

---

## Horizontal line

Horizontal lines are used to visually separate sections within a document to provide a clear break. Insert a horizontal line by putting three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

***Syntax***

```markdown
***

---

___
```

---

***Rendered Output***

***

---

___

It is best practice to add a blank line before and after a horizontal line for compatibility.

---

[back to top](#markdown-basics)

---

## Links

### Create a link

GitHub automatically create a clickable link when a valid URL is entered displaying the entire URL. However, if you would like to display text instead of the URL, you can do so by enclosing the text you would like to be displayed in square brackets ( [ ] ) followed by the URL in round brackets ( ( ) ).

***Syntax***

```markdown
https://github.com/krauseannelize

[My Github page](https://github.com/krauseannelize)
```

---

***Rendered Output***

https://github.com/krauseannelize

[My Github page](https://github.com/krauseannelize)

---

[back to top](#markdown-basics)

---

### Reference links

When you need to refer to the same URL multiple times, you can use reference links to create links that refer to specific definitions. You can do this by placing the definition in square brackets ( [ ] ), followed by a colon ( \: ), a space and then the URL as is or enclosing it in left and right angle brackets ( < > ). Refer to the reference link by inserting the text you would like to display in square brackets ( [ ] ) followed by round brackets ( ( ) ) containing the definition.

***Syntax***

```markdown
[my-github]: <https://github.com/krauseannelize>

See what I've been up to on Github [here](my-github).

Using the same definition [again](my-github).
```

---

***Rendered Output***

[my-github]: <https://github.com/krauseannelize>

See what I've been up to on Github [here](../my-github).

Using the same definition [again](../my-github).

---

[back to top](#markdown-basics)

---

### Add tooltips

You can display a handy tooltip when someone hovers over the link with a mouse by adding the tooltip you would like to display in quotation marks ( " " ) following the URL in the round brackets ( ( ) ).

***Syntax***

```markdown
[My Github page](https://github.com/krauseannelize "See what I've been up to!")
```

---

***Rendered Output***

[My Github page](https://github.com/krauseannelize "See what I've been up to!")

---

[back to top](#markdown-basics)

---

### Convert URLs or email addresses to links

You can turn a URL or email address into a clickable link by enclosing it in left and right angle brackets ( < > ).

***Syntax***

```markdown
<email@example.com>
```

---

***Rendered Output***

<email@example.com>

---

[back to top](#markdown-basics)

---

## Images

To add an image, add an exclamation mark (!), followed by alt text in square brackets ( [ ] ) and the path or URL to the image in round brackets ( ( ) ). in parentheses. An optional title that will be displayed when you hover over the image with a mouse can be added by inserting the text in quotation marks ( " " ) following the URL in the round brackets ( ( ) ).

Always provide descriptive alt text within the square brackets for accessibility. This text will be displayed if the image cannot be loaded.

---

***Syntax***

```markdown
Image stored in repository's root directory:

![The Octocat](/octocat.png "The Octocat")

Image stored in a subdirectory of the repository:

![The Octocat](/images/octocat.png "The Octocat")

Image inserted from a URL:

![The Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png?v8 "The Octocat")
```

---

<a name="octocat-images"></a>

***Rendered Output***

Image stored in repository's root directory:

![The Octocat](/octocat.png "The Octocat")

Image stored in a subdirectory of the repository:

![The Octocat](/images/octocat.png "The Octocat")

Image inserted from a URL:

![The Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png?v8 "The Octocat")

---

[back to top](#markdown-basics)

---

## Lists

Markdown allows you to create both ordered and unordered lists, which can be combined to create nested lists. Additionally, you can create a list with checkboxes that can be checked or unchecked to keep track of tasks.

### Ordered lists

Create an ordered list by starting each new line item with a number followed by a period. As long as you start with 1, the rest of the list _does not have to be entered in numerical order_. For compatibility, only use periods and do not use brackets.

***Syntax***

```markdown
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

---

***Rendered Output***

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

---

[back to top](#markdown-basics)

---

### Unordered lists

Create an unordered list of items without a specific order or numbering system by starting each new line item with either an asterisk (*), a dash (-), or a plus sign (+). For compatibility, do not mix and match symbols in the same list and use one symbol per list.

If you need to start an unordered list item with a number followed by a period, you can use a backslash (\\) before the number to escape the formatting.

***Syntax***

```markdown
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

---

***Rendered Output***

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

---

[back to top](#markdown-basics)

---

### Nested lists

You can combine both ordered and unordered lists to create nested lists by indenting one or more line items with four spaces or one tab. You cannot create a numbered nested list with indentation. Indentation will change the bullet character up to 3 times and you do not have to mix and match symbols. It is best practice not to indent more than 2 times.

***Syntax***

```markdown
1. Numbered line item 1
   - Bulleted line item 1
   - Bulleted line item 2
      - Nested bulleted line item
         - Sub-nested bulleted line item
2. Numbered line item 2
3. Numbered line item 3
```

---

***Rendered Output***

1. Numbered line item 1
   - Bulleted line item 1
   - Bulleted line item 2
      - Nested bulleted line item
         - Sub-nested bulleted line item
2. Numbered line item 2
3. Numbered line item 3

---

[back to top](#markdown-basics)

---

### Task lists

Keep track of tasks with checked or unchecked boxes by creating a task list. Add a dash (-) followed by  square brackets containing a space ([ ]) to the beginning of the task list item. This will create an unchecked box. To create a checked box, replace the space in the square brackets with an x ([x]).

***Syntax***

```markdown
- [ ] Task item 1
- [x] Task item 2
- [ ] Task item 3
```

---

***Rendered Output***

- [ ] Task item 1
- [x] Task item 2
- [ ] Task item 3

---

[back to top](#markdown-basics)

---

## Blockquotes

Blockquote is used when you need to highlight important text, cite a source, quote someone or create a dialogue. Create a blockquote by starting a paragraph with a right angle bracket (>). A blockquote can contain multiple paragraphs by starting each paragraph and blank line between the paragraphs with a right angle bracket. Nested blockquotes can be created by using multiple right angle brackets to indent. It is best practice to add a blank line before and after blockquotes for compatibility.

***Syntax***

```markdown
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

---

***Rendered Output***

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

[back to top](#markdown-basics)

---

## Tables

Information can be displayed in a neat and organized fashion by arranging it in rows and columns to create a table.

### Creating tables

Start and end every row with a pipe (|) for compatibility and use a pipe to separate each column. To create a column header, use three or more dashes (---). For a table to render correctly, you must include a blank line before the table and include a header row. You can add additional spaces to align the input for readability, but the rendered output will look the same without it.

***Syntax***

```markdown
Table with additional spaces:

| Header 1 | Header 2 | Header 3 |
| ---      | ---      | ---      |
| Item 1   | Item 2   | Item 3   |

Table without additional spaces:

| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Item 1 | Item 2 | Item 3 |
```

---

***Rendered Output***

Table with additional spaces:

| Header 1 | Header 2 | Header 3 |
| ---      | ---      | ---      |
| Item 1   | Item 2   | Item 3   |

Table without additional spaces:

| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Item 1 | Item 2 | Item 3 |

---

[back to top](#markdown-basics)

---

### Table alignment

By default, the table will align all text in the table to the left. You can change the alignment in the row that creates the header with three or more dashes (---) by adding a colon ( \: ) to the:

- left for left alignment ( :--- )
- right for right alignment ( ---: )
- left and right for center alignment ( :---: )

***Syntax***

```markdown
| Left | Center | Right |
| :--- | :---: | ---: |
| alignment | alignment | alignment |
| item | item | item |
```

---

***Rendered Output***

| Left | Center | Right |
| :--- | :---: | ---: |
| alignment | alignment | alignment |
| item | item | item |

---

[back to top](#markdown-basics)

---

### Formatting text inside tables

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
- [Blockquotes](#blockquotes)
- {code blocks, or HTML tags}

---

[back to top](#markdown-basics)

---

## Cross-referencing

### Referencing document sections

You can link directly to any section in a document that has a heading. Add the text you want to display in square brackets ( [] ). In round brackets ( () ) directly following the square brackets, insert a hash ( # ) and the name of the heading. The heading name will adhere to the following rules:

- it will be converted to lower case, e.g. `The START` can be referred to as `#the-start`
- spaces are replaced by a dashes ( - ), e.g. `heading basics` can be referred to as `#heading-basics`
- other punctuation and special characters will be removed, e.g. `One & Two` can be referred to as `#one--two`
- emphasis styling will be removed - for readability and consistency it is discouraged to use additional emphasis with headings

In VS Code when you type a hash inside the round bracket that follows square brackets, a dropdown list will appear and you can select from the available headings.

***Syntax***

```markdown
[refer to Headings](#headings)
```

---

***Rendered Output***

[refer to Headings](#headings)

---

[back to top](#markdown-basics)

---

### Custom anchors

Reference to another part of the document by inserting an anchor point and inserting a link to that anchor point. It is useful to place the anchor point right before the section in the document it is referring to. An anchor point was inserted in the Images section above with this syntax: `<a name="octocat-images"></a>`. Click on the link in the Rendered Output section below to see if it takes you there.

***Syntax***

```markdown
Check out the [Octocat](#octocat-images) above.
```

---

***Rendered Output***

Check out the [Octocat](#octocat-images) above.

---

[back to top](#markdown-basics)

---
