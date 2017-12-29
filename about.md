---
layout: page
title: درباره ما
permalink: /about/
---
<ul class="user-list">
{% for item in site.translators %}
  <li class="user-list__item">
        <img class="user-list__avatar" style="background-image: url(http://gravatar.com/avatar/{{ item.email | downcase | md5 }}?s=100); background-size:cover;">
        <div class="user-list__name">{{item.name}}</div>
        <div class="user-list__address">{{item.email | downcase}}</div>
  </li>
{% endfor %}
</ul>

