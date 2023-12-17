---
title: Mermaid Support
date: 2023-12-17T20:26:13Z
description: ""
slug: ""
authors:
  - John Doe
  - Jane Doe
tags:
  - mermaid
  - hugo
  - markdown
  - css
  - html
categories:
  - theme demo
  - syntax
externalLink: ""
series:
  - Theme Demo
draft: false
weight: 20
featuredImage: ""
---

If you want to use [Mermaid-JS](https://mermaid-js.github.io/mermaid/#/) on your website.
Provide `mermaid` as [Shortcode](https://gohugo.io/content-management/shortcodes/#readout) in your markdown file.

{{<mermaid>}}
flowchart LR

    A --> C

    B --> A

    C --> D

    D --> B

{{</mermaid>}}

{{<mermaid>}}
sequenceDiagram
Alice->>John: Hello John, how are you?
loop Healthcheck
John->>John: Fight against hypochondria
end
Note right of John: Rational thoughts!
John-->>Alice: Great!
John->>Bob: How about you?
Bob-->>John: Jolly good!
{{</mermaid>}}

Find more example on [Mermaid-JS](https://mermaid-js.github.io/mermaid/#/) website.
