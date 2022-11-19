---
title: "Tags"
description: "All of my blog posts sorted by tag"
permalink: /blog/tags
---

{% include search.html %}

<h2 id="categories">Categories</h2>
<div class="tag-list">
<a href="/blog">Essays ({{ site.categories.essays | size }})</a>
<a href="/blog/now">Now ({{ site.categories.now | size }})</a>
<a href="/notes">Recent notes</a>
</div>

<h2 id="tags">Tags</h2>

{% assign sortedTags = site.tags | sort %}

<div class="tag-list">
{% for tag in sortedTags %}
	<a href="#{{tag[0]}}">{{ tag[0] }}&nbsp;({{ tag[1] | size }})</a>
{% endfor %}
</div>

{% for tag in sortedTags %}

<section class="posts-by-tag">

<h2 id="{{ tag[0] }}">{{ tag[0] }}</h2>

{% for post in tag[1] %}
	{% include blog-listing.html %}
{% endfor %}

<p><a href="#" class="internal-link">All Tags &#8593;</a></p>

{% endfor %}
