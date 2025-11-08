---
title: Callout
description:
permalink:
lang: en-US
publish:
draft:
enableToc:
tags:
aliases:
cssclasses:
socialDescription:
socialImage:
created: 2025-11-07
modified: 2025-11-07
published: 2025-11-07
---
Callout blocks, sometimes called "admonitions", are written as a blockquote.

The following syntax denote a callout block: `> [!INFO]`.

```markdown
> [!INFO]
> Here's a callout block.
> It supports **markdown** and [[Internal link|wikilinks]].
```

It will show up like this:
> [!INFO]
> Here's a callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

### Types

There are 12 distinct callout types, each with several aliases. Each type comes with a different background color and icon.

To use these default styles, replace `INFO` in the examples with any of these types. Any unrecognized type will default to the "note" type, unless they are [[#Customizations|customized]]. The type identifier is case insensitive.

- note
- abstract, summary, tldr
- info, todo
- tip, hint, important
- success, check, done
- question, help, faq
- warning, caution, attention
- failure, fail, missing
- danger, error
- bug
- example
- quote, cite

> [!NOTE]
> Here's an info callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!ABSTRACT]
> Here's an abstract callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!SUMMARY]
> Here's a summary callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!TLDR]
> Here's a TLDR callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!TODO]
> Here's a To do callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!TIP]
> Here's a tip callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!HINT]
> Here's a hint callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!IMPORTANT]
> Here's an important callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!SUCCESS]
> Here's a success callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!CHECK]
> Here's a check callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!DONE]
> Here's a done callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!QUESTION]
> Here's a question callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!HELP]
> Here's a help callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!FAQ]
> Here's a FAQ callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!WARNING]
> Here's a warning callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!CAUTION]
> Here's a caution callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!ATTENTION]
> Here's an attention callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!FAILURE]
> Here's a failure callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!FAIL]
> Here's a fail callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!MISSING]
> Here's a missing callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!DANGER]
> Here's a danger callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!ERROR]
> Here's an error callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!BUG]
> Here's a bug callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!EXAMPLE]
> Here's an example callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!QUOTE]
> Here's a quote callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

> [!CITE]
> Here's a cite callout block.
> It supports **markdown** and [[VRT/Formatting/Internal link|wikilinks]].

### Title and body

You can define the title of the callout block, and you can also have a callout without body content.

```markdown
> [!TIP] Callouts can have custom titles, which also supports **markdown**!
```

> [!TIP] Callouts can have custom titles, which also supports **markdown**!

### Folding

Additionally, you can create a folding callout by adding `+` (default expanded) or `-` (default collapsed) after the block.

```markdown
> [!FAQ]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden until it is expanded.
```

Will show up as:

> [!FAQ]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden until it is expanded.

### Customizations

Snippets and plugins can define custom callouts too, or overwrite the default options. Callout types and icons are defined in CSS, where the color is an `r, g, b` tuple and the icon is the icon ID from any internally supported icon (like `lucide-info`). Alternatively, you can specify an SVG icon as a string.

```CSS
.callout[data-callout="my-callout-type"] {
    --callout-color: 0, 0, 0;
    --callout-icon: icon-id;
    --callout-icon: '<svg>...custom svg...</svg>';
}
```

For example:
```CSS
.callout[data-callout="minimal-callout"] {
    --callout-color: transparent;
    border: none;
    --callout-icon: pen-tool;
}

.callout[data-callout="minimal-callout"] .callout-content {
    text-align: center;
}

```

```
> [!minimal-callout] A Generic Title
> Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus assumenda iusto sint officia quas distinctio doloribus harum optio commodi eum!
```

> [!minimal-callout] A Generic Title
> Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus assumenda iusto sint officia quas distinctio doloribus harum optio commodi eum!
