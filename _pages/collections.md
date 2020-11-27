---
title: Collections

---

<h2>Sim Racing</h2>

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in site.posts %}
    {% if post.path contains 'simracing' %}
        {% include archive-single.html type=entries_layout %}
    {% endif %}
  {% endfor %}
</div>

<h2>Builds</h2>

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in site.posts %}
    {% if post.path contains 'builds' %}
        {% include archive-single.html type=entries_layout %}
    {% endif %}
  {% endfor %}
</div>

<h2>Analytics</h2>

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in site.posts %}
    {% if post.path contains 'analytics' %}
        {% include archive-single.html type=entries_layout %}
    {% endif %}
  {% endfor %}
</div>

{% include paginator.html %}
