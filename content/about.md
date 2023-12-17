---
title: "About Me"
date: 2023-09-30T13:36:31-06:00
aliases:
  - info
  - about
  - about-me
  - need-to-know
draft: false
featuredImage: ""
---

this is were the content goes for the about page and/or contact page. If the contact page is not needed, then delete the option in the config.yaml file.

Turning this:

```yaml
menu:
  main:
    - name: Posts
      weight: 1
      url: /posts/
    - name: Projects
      weight: 2
      url: projects/
    - name: Wiki
      weight: 3
      url: wiki/
    - name: About
      weight: 4
      url: /about/
```

Into this:

```yaml
menu:
  main:
    - name: Posts
      weight: 1
      url: /posts/
    - name: Projects
      weight: 2
      url: projects/
    - name: Wiki
      weight: 3
      url: wiki/
```
