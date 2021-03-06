---
layout: page
title: Writing list
headline: Things I'd like to write about
permalink: /writing-list
---

I often get <i class="fa fa-lightbulb-o"></i> ideas popping into my head. At the time they seem pretty urgent and sometimes even amazing ideas that I want to explore and write about. However, it's pretty tough to get anything <i class="fa fa-check-square-o"></i> done these days, for one reason or another.
So, I keep my ideas here, so that I can come back to them every so often and see if maybe I can get around to writing about them.

<hrule>
<div class="col-md-6">
<ul class="fa-ul">
{% comment %} {{ site.data.todo.first.date }} {% endcomment %}
{% for item in site.data.todo %}
  {% unless item.done %}
  <li><i class="fa-li fa fa-lightbulb-o"></i> <strong>{{ item.title }}</strong> - {{ item.description }}</li>
  {% endunless %}
{% endfor %}
</ul>
</div>
<div class="col-md-6">
<ul class="fa-ul">
{% for item in site.data.todo %}
{% if item.done %}
  <li><i class="fa-li fa fa-check-square-o"></i> <strong>{{ item.title }}</strong> - {{ item.description }} ({{ item.date | date: '%b %d, %Y'}})</li>
{% endif %}
{% endfor %}
</ul>
</div>
