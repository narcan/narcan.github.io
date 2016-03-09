---
layout: page
title: Stories
subtitle: A Collection of Strange Sagas
---
<div id="stories_page">
  <p>
    <span class="author ar">by Pedro Ávila
  </p>
  
  <ul class="story_list">
    {% for story in site.menu %}
      {% if menu_item.title %}
        <div class=“page-link“ href="{{ menu_item.url | prepend: site.baseurl }}">{{ menu_item.title }}</div>
        <span class="">{{ story.description }}</span>
      {% endif %}
    {% endfor %}

    {% for story in site.stories %}
    <li>
        <h4><a class="story_title" href="{{ story.url | prepend: site.baseurl }}">{{ story.title }}</a></h4>
        <span class="story_description">{{ story.description }}</span>
    </li>
    {% endfor %}
  </ul>
  
  <div class="copyright">
    <a href="{{ '/about/copyright/' | prepend: site.baseurl }}">&copy; 2009 Pedro Ávila</a>
  </div></p>
</div>