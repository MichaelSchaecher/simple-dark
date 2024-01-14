---
title: Image Management
# Set date to Mountain Standard Time. Example: 2023-12-17T20:01:00-07:00
date: 2023-12-21T21:19:23-07:00
description: ""
slug: ""
authors:
  - Michael Schaecher
tags:
  - images
  - scss
  - shortcodes
categories:
  - images control
externalLink: ""
series:
draft: false
weight: 20
featuredImage: "https://clipart-library.com/newimages/camera-clipart-4.jpg"
---

Hugo comes with a built-in shortcode for images that allows for adding captions and resizing images. This is useful for adding images to your content without having to worry about aligning the images and adding captions.

With the add styling from [Simple Dark](https://github.com/MichaelSchaecher/simple-dark) you can also align the images to the left, center, or right.

> **Tip**: The src path is an absolute path from the root of the site. This means that the full path to the image is required. For example, if your image is located at `static/images/image.png` then the src path would be `/images/image.png`. If your image is located in the same directory as your content then the src path would be `./image.png`.

## Left Alignment

{{< highlight html >}}
{{</* figure class="left" src="./left.png" caption="This is a left aligned image" */>}}
{{< /highlight >}}

{{< figure class="left" src="./left.png" caption="This is a left aligned image" >}}

## Center Alignment

{{< highlight html >}}
{{</* figure class="center" src="./center.png" caption="This is a center aligned image" */>}}
{{< /highlight >}}

{{< figure class="center" src="./center.png" caption="This is a right aligned image" >}}

## Right Alignment

{{< highlight html >}}
{{</* figure class="right" src="./right.png" caption="This is a right aligned image" */>}}
{{< /highlight >}}

{{< figure class="right" src="./right.png" caption="This is a right aligned image" >}}
