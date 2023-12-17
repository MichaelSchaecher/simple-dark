---
title: Math Typesetting
date: 2023-12-17T20:04:23Z
description: ""
slug: ""
authors:
  - John Doe
  - Jane Doe
tags:
  - math
  - latex
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

Mathematical notation in a Hugo project can be enabled by using third party JavaScript libraries.

<!--more-->

In this example we will be using [KaTeX](https://katex.org/)

- Create a partial under `/layouts/partials/math.html`
- Within this partial reference the [Auto-render Extension](https://katex.org/docs/autorender.html) or host these scripts locally.
- Include the partial in your templates like so:

```bash
{{ if or .Params.math .Site.Params.math }}
{{ partial "math.html" . }}
{{ end }}
```

- To enable KaTex globally set the parameter `math` to `true` in a project's configuration
- To enable KaTex on a per page basis include the parameter `math: true` in content files

**Note:** Use the online reference of [Supported TeX Functions](https://katex.org/docs/supported.html)

## Examples

Simple addition and subtraction:

$$
  a + b = c
$$

$$
  a - b = c
$$

Simple multiplication and division:

$$
  a \times b = c
$$

$$
  \frac{a}{b} = c
$$

Fractions:

$$
  \frac{a + b}{c + d} = e
$$

the quadratic formula:

$$
  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

Block math:

$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots}}}
$$
