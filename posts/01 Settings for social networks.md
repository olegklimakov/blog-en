---
title: How to improve your website for social networks
description: Simple ways to make your website a little better
date: 2021-07-26
tags:
- Tech
- Social
- Notes
layout: layouts/post.njk
permalink: "/how-to-update-preview-in-telegram/"
image: https://sun9-35.userapi.com/impg/jiskIOUD3dPjI60BBMmJkEZIc_HMh3EX_dMbbQ/TAYxLfmn970.jpg?size=640x360&quality=96&sign=8db726a8e4d68108d78a345efe66fa10&type=album
---
# Website settings

## Motivation

It is better to have fancy preview, when somebody will share the link of your website.
Like this (in Facebook):

![](https://paper-attachments.dropbox.com/s_91EF3957196186B634A16DEEC8E589063D47D4DC65B0E0C15FA2D525B2C8778A_1627562229354_++2021-07-29++15.36.00.png)



## How to achieve it?

It is not difficult. You just need to update your index.html file.
Inside `<head>`:

- For description. You need to add  `<meta content="Description for your website" property="og:description">`
- For image preview `<meta content="link to your image" property="og:image">`
- For website name `<meta content="Website name" property="og:title">`

Example:

    <html>
      ...
      <head>
        <meta property="og:title" content="Page or website title">
        <meta property="og:description" content="Description">
        <meta property="og:image" content="{{ image | absoluteUrl(metadata.url) }}">
      </head>
      ...
    </html>


# Problem solving
## Telegram:

There are some cases when you changed or add this information, but you still see the old version.
In that case you need a [special bot](https://t.me/WebpageBot). Just send it a link to your website.

