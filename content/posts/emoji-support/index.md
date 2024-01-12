---
title: Emoji Support
date: 2023-12-17T21:39:12Z
lastmod: 2023-12-17T21:39:12Z
description: ""
slug: ""
authors:
  - John Doe
  - Jane Doe
tags:
  - text
  - markdown
  - emoji
categories:
  - Placeholder
externalLink: ""
series:
  - Theme Demo
draft: false
weight: 20
featuredImage: ""
---

Emoji can be enabled in a Hugo project in a number of ways.

<!--more-->

The [`emojify`](https://gohugo.io/functions/emojify/) function can be called directly in templates or [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

To enable emoji globally, set `enableEmoji` to `true` in your site's [configuration](https://gohugo.io/getting-started/configuration/) and then you can type emoji shorthand codes directly in content files; e.g.

For better emoji support install the pluging for VSCode [vscode-emoji](https://marketplace.visualstudio.com/items?itemName=bierner.emojisense).

````html
```html 🙈 `:see_no_evil:` 🙉 `:hear_no_evil:` 🙊 `:speak_no_evil:`

<br />

The [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) is a useful reference
for emoji shorthand codes. --- **N.B.** The above steps enable Unicode Standard
emoji characters and sequences in Hugo, however the rendering of these glyphs
depends on the browser and the platform. To style the emoji you can either use a
third party emoji font or a font stack; e.g. {{< highlight css >}} .emoji {
font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol,
Android Emoji, EmojiSymbols; } {{< /highlight >}} {{< highlight html >}}

<style>
  .emojify {
    font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji,
      Segoe UI Symbol, Android Emoji, EmojiSymbols;
    font-size: 2rem;
    vertical-align: middle;
  }
  @media screen and (max-width: 650px) {
    .nowrap {
      display: block;
      margin: 25px 0;
    }
  }
</style>

{{< /highlight >}}
````
