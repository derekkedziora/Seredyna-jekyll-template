---
title: "How to post"
description: "An example post"
category: essays
tags: optional example
permalink: /blog/how-to-post
date: 2022-11-12 09:48
syntax: true
---

To make a regular blog post, use this YAML head matter: 

```
---
title: "How to post"
description: "An example post"
category: essays
tags: optional example
permalink: /blog/how-to-post
date: 2022-11-12 09:48
---
```

A post must have to the the category `essay` in order to appear in the post list on the `/blog` page. 

Adding tags is optional. They will automatically update on the `/blog/tags` page with each build. 

If you want syntax highlighting in a post add `syntax: true` to the YAML front matter. This triggers the syntax CSS file to load. 