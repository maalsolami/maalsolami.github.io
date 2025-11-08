---
title: Paragraphs
description:
permalink:
lang:
publish: true
draft:
enableToc: true
tags:
aliases:
cssclasses:
socialDescription:
socialImage:
created: 2025-11-08
modified: 2025-11-08
published: 2025-11-08
---
A blank lines can be used to separate blocks of text to create paragraphs in Markdown. Each block of text separated by a blank line is treated as a distinct paragraph.

```md
This is a paragraph.

This is another paragraph.
```

This is a paragraph.

This is another paragraph.

A blank line between lines of text creates separate paragraphs. This is the default behavior in Markdown.

### Multiple blank spaces
Multiple adjacent blank spaces within and between paragraphs collapse into a single space when rendered and displayed.

```md
Multiple          adjacent          spaces



and multiple newlines between paragraphs.
```

Multiple          adjacent          spaces



and multiple newlines between paragraphs.

If you want to prevent spaces from collapsing or add multiple blank spaces, you can use the `&nbsp;` (non-breaking space) or `<br>` (line break) HTML tags.

```md
Multiple&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;adjacent&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;spaces
<br>
<br>
<br>
and multiple newlines between paragraphs.
```

Multiple&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;adjacent&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;spaces
<br>
<br>
<br>
and multiple newlines between paragraphs.

### Line breaks
In Markdown, a single `Enter` is ignored, and multiple consecutive `Enter` presses result in just one new paragraph. This behavior aligns with Markdown’s soft wrap rule, where extra blank lines do not generate additional line breaks or paragraphs—they are collapsed into a single paragraph break. This is how Markdown handles text by default, ensuring that paragraphs flow naturally without unexpected breaks​.

In some Markdown editors, pressing `Enter` once will create a new line in your note, but it is treated as a _continuation_ of the same paragraph in the rendered output, following typical Markdown behavior. To insert a line break _within_ a paragraph without starting a new paragraph, you can either:
- Add two spaces at the end of a line before pressing Enter, or
- Use the shortcut Shift + Enter to directly insert a line break. 