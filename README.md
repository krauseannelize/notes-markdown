# Guide to Markdown
This is my own notes to provide a quick reference guide on writing documentation in Markdown.
## Contents
1. [Paragraphs](#paragraphs)
2. [Headings](#headings)
3. [Cross-Referencing](#cross-referencing)

---

<a name="paragraphs" />

## Paragraphs

Create paragraphs by entering text without any symbols. Remember to use a blank line to separate one or more lines of text.

**Input:**

```
Text line 1

Text line 2
```

**Output:**

Text line 1

Text line 2

---

<a name="headings" />

## Headings

To create a heading, add the hash symbol (#) in front of the heading text. The number of
hash symbols correspond to the heading level and you can have up to 6 heading levels. Remember to add a space between the hash symbol and the text for ensure compatibility.

**Input:**

```
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6
```

**Output:**

# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6

---

<a name="cross-referencing" />

## Cross-referencing

Reference to another part of the document by inserting an anchor point and inserting a link to that anchor point. It is useful to place the anchor point right before the section in the document it is referring to.

**Input:**

```
Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

### Anchor Point
```

**Output:**


Reference to [Anchor Point](#anchor-point).

<a name="anchor-point" />

### Anchor Point

---