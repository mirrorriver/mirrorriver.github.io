---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home

---




<div class="listing">
    {% for post in site.posts %}
    <article> 
        <header class="entry-header">
            <h2 class="entry-title">
            <!-- a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a -->
            {{ post.title }}
            </h2>
            <time class="published" datetime="{{ post.date }}" pubdate="">
            <!-- a href="{{ post.url | prepend: site.baseurl }}">{{ post.date | date: '%B %d, %Y' }}</a -->
            {{ post.date | date: '%B %d, %Y' }}
            </time>
        </header>
        <div class="entry-content">
            {{ post.content }}
        </div>
    </article>
    {% endfor %}
</div>