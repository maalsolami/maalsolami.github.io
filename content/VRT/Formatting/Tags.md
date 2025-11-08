---
title: Tags
description:
permalink:
lang:
publish: true
draft:
enableToc: true
tags:
  - metadata
  - search
aliases:
cssclasses:
socialDescription:
socialImage:
created: 2025-11-08
modified: 2025-11-08
published: 2025-11-08
---
Tags are keywords or topics that help you quickly find the documents you want.

## Add a tag
Tags can be added to a document by entering in the editor a hash symbol (#) followed by a keyword. For example, #project.

Tags can also be added using the tags property of the document. Tags in the tags property are often in YAML and formatted as a list:

```yaml
tags:
	- metadata
	- search
```

## Nested tags
Nested tags define tag hierarchies that make it easier to find and filter related tags.

Nested tags can be created by using forward slashes (`/`) in the tag name, for example #project/planning and #project/execution

## Tag format
The following are some of the common rules for formatting tags. The following characters can be used:
- Alphabetical letters
- Numbers
- Underscore (`_`)
- Hyphen (`-`)
- Forward slash (`/`) for [[VRT/Formatting/Tags#Nested tags|Nested Tags]]

Tags must contain at least one non-numerical character. For example, #1984 isn't a valid tag, but `#y1984` is.

Tags are case-insensitive. For example, `#tag` and `#TAG` will be treated as identical.

Tags can't contain blank spaces. To separate two or more words, you can instead use the following formats:
- `#camelCase`
- `#PascalCase`
- `#snake_case`
- `#kebab-case`
