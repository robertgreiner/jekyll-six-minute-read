---
layout: page
title: Robert Greiner
tagline: 
---

<div>
	{% for page in site.posts limit:3 %}
		<article class="post">
			<h1 class="post-title"><a href="{{ BASE_PATH }}{{ page.url }}">{{ page.title }}</a></h1>
	    	<div class="post-date"><span>Written by <a href="/about">Robert Greiner</a></span> on <span class="date">{{ page.date | date: "%B %d, %Y" }}</span></div>
            <div class="post-meta"><span>{{ page.content | number_of_words | plus: 300 | divided_by: 160 | append: " minute read" }}</span></div>
	    	<div class="clear"></div>
	    	<div>{{ page.content }}</div>
	    	<div class="clear"></div>
		</article>
	{% endfor %}
</div>

<div style="margin: 10px 0 20px 0;">
<a href="/archive.html">More Posts</a>
</div>