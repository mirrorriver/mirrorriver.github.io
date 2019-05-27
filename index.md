---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home

---




Thanks for stopping by and I'm glad you could make it. This is the primary web site for William O'Neill. You can learn more about me on the [about page](/about/).

## Posts

<ul>
  {% for post in site.posts %}
    
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    
      
   
  {% endfor %}
</ul>
