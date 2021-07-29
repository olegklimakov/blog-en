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
When you share your website in social networks, I guess you want to do it the best way - with description, site title and image (like on the example from facebook). It allows to your visitor to check common information before visiting and be ready that this link is about something serous, and not about cat gifs (unfortunately).

![](https://paper-attachments.dropbox.com/s_91EF3957196186B634A16DEEC8E589063D47D4DC65B0E0C15FA2D525B2C8778A_1627562229354_++2021-07-29++15.36.00.png)


How to achieve it? It is not difficult, but you need to update your html file.

- For description. You need to add inside `<head>` tag `<meta content="Description for your website" property="og:description">`
- For image preview `<meta content="link to your image" property="og:image">`
- For website name `<meta content="Website name" property="og:title">`
# Problem solving
## Telegram:

There are some cases when you changed or add this information, but you still see the old version.
In that case you need a [special bot](https://t.me/WebpageBot). Just send him a link to your website.

