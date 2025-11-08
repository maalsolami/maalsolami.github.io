---
title: Embed Web Pages
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
Learn how to use the [iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe) HTML element to embed web pages in your notes.

To embed a web page, add the following in your note and replace the placeholder text with the URL of the web page you want to embed:

```html
<iframe src="INSERT YOUR URL HERE"></iframe>
```

```md
<iframe id="net.daringfireball.markdown"
    title="The initial description of Markdown"
    width="768"
    height="1024"
    src="https://daringfireball.net/projects/markdown/">
</iframe>
```

<iframe id="net.daringfireball.markdown"
    title="The initial description of Markdown"
    width="768"
    height="1024"
    src="https://daringfireball.net/projects/markdown/">
</iframe>


>[!NOTE]
>Some websites don't allow you to embed them. Instead, they may provide URLs that are meant for embedding them. If the website doesn't support embedding, try searching for the name of the website followed by "embed iframe". For example, "youtube embed iframe".
