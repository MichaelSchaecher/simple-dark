---
title: Html and Css Only Tabs
date: 2023-12-16T23:28:19Z
description: ""
slug: ""
authors:
  - John Doe
  - Jane Doe
tags:
  - html
  - css
categories:
  - html
externalLink: ""
series:
draft: false
weight: 20
featuredImage: ""
---

## Shortcodes

The following content:

```markdown
{{</* tabgroup */>}}
{{</* tab name="Hello" */>}}
Hello World!
{{</* /tab */>}}

{{</* tab name="Goodbye" */>}}
Goodbye Everybody!
{{</* /tab */>}}
{{</* /tabgroup */>}}
```

Will generate:

{{< tabgroup >}}
{{< tab name="Hello" >}}
Hello World!
{{< /tab >}}

{{< tab name="Goodbye" >}}
Goodbye Everybody!
{{< /tab >}}
{{< /tabgroup >}}

## Right alighment

You can also align the tabs to the right:

```markdown
{{</* tabgroup align="right" */>}}
{{</* tab name="Hello" */>}}
Hello World!
{{</* /tab */>}}

{{</* tab name="Goodbye" */>}}
Goodbye Everybody!
{{</* /tab */>}}
{{</* /tabgroup */>}}
```

Giving you this look:

{{< tabgroup align="right" >}}
{{< tab name="Hello" >}}
Hello World!
{{< /tab >}}

{{< tab name="Goodbye" >}}
Goodbye Everybody!
{{< /tab >}}
{{< /tabgroup >}}

## Markdown content

Any valid markdown can be used inside the tab:

````markdown
{{</* tabgroup align="right" style="code" */>}}
{{</* tab name="toml" */>}}

```toml
[params]
puts = 'Hello'
```

{{</* /tab */>}}
{{</* tab name="yaml" */>}}

```yaml
params:
  puts: "Hello"
```

{{</* /tab */>}}
{{</* tab name="json" */>}}

```json
{
  "params": {
    "puts": "Hello"
  }
}
```

{{</* /tab */>}}
{{</* /tabgroup */>}}
````

And you get this lovely content:

{{< tabgroup align="right" style="code" >}}
{{< tab name="toml" >}}

```toml
[params]
puts = 'Hello'
```

{{< /tab >}}
{{< tab name="yaml" >}}

```yaml
params:
  puts: "Hello"
```

{{< /tab >}}
{{< tab name="json" >}}

```json
{
  "params": {
    "puts": "Hello"
  }
}
```

{{< /tab >}}
{{< /tabgroup >}}

In this case `style="code"` makes it look a little nicer for scenarios where
your content is purely a code block.
