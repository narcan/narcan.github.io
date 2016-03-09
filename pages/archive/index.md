---
layout: page
---
*   <span class="post-teaser__date">
		{{ post.date | date: "%d %B %Y" }} --- {{ post.location }}
	</span>

    ## [<span class="post-teaser__title">{{ post.title }}</span>]({{ post.url | prepend: site.baseurl }})

    <span class="post-teaser__excerpt">{{ post.excerpt }}</span>