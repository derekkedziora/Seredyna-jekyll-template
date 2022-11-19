---
title: Contact
description: "Email is the best way to get in touch."
permalink: /contact
--- 



Email’s the best way to get in touch: 

**{{ site.email }}**

<div class="tag-list copy-buttons">

<button class="btn btn-default" onclick="copyEmailtoClipboard('{{site.email}}')">Copy address</button>

<a href="mailto:{{site.email}}">Send email</a>
</div>

Add some social media or other ways to follow you.

[RSS](/rss) is the best way to follow me.

<script>

// copy email to clipboard

function copyEmailtoClipboard() {
    navigator.clipboard.writeText((arguments[0]));
}

</script>