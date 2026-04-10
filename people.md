---
layout: page
title: People
subtitle: Group members past and present
menu: main
---

{% for member in site.members.present %}
<div class="member">
  <img class="member-photo" src="{{ member.image }}" alt="{{ member.name }}">
  <div class="member-info">
    <h3>{{ member.name }}</h3>
    {% if member.position %}<p><em>{{ member.position }}</em></p>{% endif %}
    <p>{{ member.description }}</p>
  </div>
</div>
{% endfor %}

## Former members

{% for member in site.members.former %}
<div class="member">
  <img class="member-photo" src="{{ member.image }}" alt="{{ member.name }}">
  <div class="member-info">
    <h3>{{ member.name }}</h3>
    <p>{{ member.description }}</p>
  </div>
</div>
{% endfor %}
