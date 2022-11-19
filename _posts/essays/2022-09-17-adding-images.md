---
title: "Adding images"
description: "Add some images to your posts" 
category: essays
tags: example
permalink: /blog/adding-images
date: 2022-09-17 21:25
syntax: true
---

I don’t use many images, so I never built a more automated system to handle them. I also don’t use a fancy CDN because I like the portability of everything being a single git repo that’s easy to migrate wherever. 

I save everything in `/static/post-content/{% raw %}{{date-of-post}/{{image-name}}{% endraw %}`

If you don’t want an image caption, the standard markdown format works: `![No dogs allowed](/static/post-content/2022-09-17/no-dogs.jpeg)`

![No dogs allowed](/static/post-content/2022-09-17/no-dogs.jpeg)

If you want to add an caption, then you have to use HTML:

 ```html
 <figure>
 <img src="/static/post-content/2022-09-17/no-dogs.jpeg"
 alt="No dogs allowed">
 <figcaption>This is a safe space for cat people</figcaption>
 </figure>
 ```

 <figure>
 <img src="/static/post-content/2022-09-17/no-dogs.jpeg" alt="No dogs allowed">
 <figcaption>This is a safe space for cat people</figcaption>
 </figure>

 And that’s it for images! 