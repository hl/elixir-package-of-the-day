---
layout: home
---

<h3>Package of the week</h3>
<h1>{{ site.data.featured_package.name }}</h1>
<p>{{ site.data.featured_package.description }}</p>
<ul>
  <li><a href="{{ site.data.featured_package.hex }}">{{ site.data.featured_package.hex }}</a></li>
  <li><a href="{{ site.data.featured_package.github }}">{{ site.data.featured_package.github }}</a></li>
</ul>

<h3>Past packages of the week</h3>

{% for package in site.data.past_packages %}
  <h2>{{ package.name }}</h2>
  <p>{{ package.description }}</p>
  <ul>
    <li><a href="{{ package.hex }}">{{ package.hex }}</a></li>
    <li><a href="{{ package.github }}">{{ package.github }}</a></li>
  </ul>
{% endfor %}
