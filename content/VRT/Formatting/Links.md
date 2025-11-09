---
title: Links
description:
permalink:
lang: en-US
publish: true
draft:
enableToc: true
tags:
aliases:
cssclasses:
socialDescription:
socialImage:
created: 2025-11-07
modified: 2025-11-08
published: 2025-11-07
---
#### External links

Markdown style links can be used to refer to either external objects, such as web pages, or an internal page or image.

```md
http://en.wikipedia.org/ - automatic conversion to a link

[Wikipedia](en.wikipedia.org/)
```

http://en.wikipedia.org/ - automatic conversion to a link

[Wikipedia](en.wikipedia.org/)

#### URI links

URI links can be used to open open and interact with  another program.

For example, you can link to a file in a vault like so (please note the required encoding):

```md
[Email John Doe](mailto:john.doe@example.com)
[Call now](tel:+1-816-555-1212)
[Map a location](geo:25.245470718844146,51.45400942457904)
[Open Wikipedia in Google Chrome](googlechrome:en.wikipedia.org/)
[Open calendar](calshow:)
```

[Email John Doe](mailto:john.doe@example.com)
[Call now](tel:+1-816-555-1212)
[Map a location](geo:25.245470718844146,51.45400942457904)
[Open Wikipedia in Google Chrome](googlechrome:en.wikipedia.org/)
[Open calendar](calshow:)

#### Escaping

If there are spaces in the url, they can be escaped by either using `%20` as a space, such as:

```md
[Format your notes](Format%20your%20notes)
```

[Format your notes](VRT/Formatting/Format%20your%20notes.md)

Or you can enclose the target in `<>`, such as:

```md
[Format your notes](<Format your notes>)
```

[Format your notes](<VRT/Formatting/Format your notes.md>)
