# Guide to Markdown

As someone who has spent two decades editing and formatting legal documents, Markdown was the logical starting point when I started to learn code and using Git. Its simplicity, readability, and versatility make it an ideal tool for writing and maintaining documentation.

This guide aims to provide a concise overview of Markdown syntax and best practices. It's primarily intended as a quick reference for myself, but I hope it will also be helpful to others who are new to Markdown or looking to refresh their knowledge.

## Contents
1. [Paragraphs](#paragraphs)
2. [Emphasis](#emphasis)
3. [Headings](#headings)
4. [Lists](#lists)
	- [Ordered lists](#lists-ordered)
	- [Unordered lists](#lists-unordered)
	- [Nested lists](#lists-nested)
5. [Cross-Referencing](#cross-referencing)

---

<a name="paragraphs" />

## Paragraphs

Create paragraphs by entering text without any symbols. Remember to use a blank line to separate one or more lines of text.

**_Input:_**

```
Text line 1

Text line 2
```

**_Output:_**

Text line 1

Text line 2

---

<a name="emphasis" />

## Emphasis

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
| Highlight | `<mark>Mark tag</mark> for highlighting` | `<mark>Mark tag</mark> for highlighting` |

---

<a name="headings" />

## Headings

To create a heading, add the hash symbol (#) in front of the heading text. The number of
hash symbols correspond to the heading level and you can have up to 6 heading levels. Remember to add a space between the hash symbol and the text for ensure compatibility.

**_Input:_** 

```
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6
```

**_Output:_**

# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6

---

<a name="lists" />

## Lists

Markdown allows you to create both ordered and unordered. You can also combine both of the lists to create nested lists.

<a name="lists-ordered" />

### Ordered lists

Create an ordered list by starting each new line item with a number followed by a period. As long as you start with 1, the rest of the list _does not have to be entered in numerical order_. For compatibility, only use periods and do not use brackets.

**_Input:_**

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

**_Output:_**



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

### Unordered lists

Create an unordered list of items without a specific order or numbering system by starting each new line item with either an asterisk (*), a dash (-), or a plus sign (+). For compatibility, do not mix and match symbols in the same list and use one symbol per list.

If you need to start an unordered list item with a number followed by a period, you
can use a backslash (\\) to escape the period.

**_Input:_**

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

**_Output:_**

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

### Nested lists

You can combine both ordered and unordered lists to create nested lists by indenting one or more line items with four spaces or one tab. You cannot create a numbered nested list with indentation and a nested list will break the automatic numbering. Indentation will change the bullet character up to 3 times and you do not have to mix and match symbols. It is best practice not to indent more than 2 times.

**_Input:_**

```
1. Numbered line item 1
* Bulleted line item
* Bulleted line item
	* Nested bulleted line item
		* Sub-nested bulleted line item
2. Numbered line item 3
3. Numbered line item 4
```

**_Output:_**

1. Numbered line item 1
* Bulleted line item
* Bulleted line item
	* Nested bulleted line item
		* Sub-nested bulleted line item
2. Numbered line item 3
3. Numbered line item 4

---

<a name="cross-referencing" />

## Cross-referencing

Reference to another part of the document by inserting an anchor point and inserting a link to that anchor point. It is useful to place the anchor point right before the section in the document it is referring to.

**_Input:_**

```
Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

### Anchor Point
```

**_Output:_**


Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

### Anchor Point

---
