---
title: {{ replace .File.ContentBaseName "-" " " | title }}
# Set date to Mountain Standard Time. Example: 2023-12-17T20:01:00-07:00
date: {{ .Date }}
lastmod: {{ .Date }}
description: ""
slug: {{ .File.ContentBaseName }}
authors:
  - {{ .Site.Params.author }}
tags:
  - new
categories:
  - new
externalLink: ""
series:
draft: true
weight: 20
featuredImage: ""
---
