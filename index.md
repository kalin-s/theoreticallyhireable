---
layout: default
title: Theoretically Hireable
---

{% for post in site.posts %}
<article>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %-e, %Y" }}{% if post.tags %} · {{ post.tags | array_to_sentence_string }}{% endif %}</p>
  <p>{{ post.excerpt }}</p>
</article>
<hr style="border:none; border-top:1px solid rgba(255,255,255,0.03); margin:1rem 0;">
{% endfor %}
