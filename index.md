---
layout: home
---

{% assign featured_package = site.packages | where: "featured", "true" | first %}

### This weeks featured package

# {{ featured_package.title }}

{{ featured_package.content }}

- [{{ featured_package.hex }}]({{ featured_package.hex }})
- [{{ featured_package.github }}]({{ featured_package.github }})

---

### Past packages of the week

{% for package in site.packages %}

## {{ package.title }}

{{ package.content }}

- [{{ package.hex }}]({{ package.hex }})
- [{{ package.github }}]({{ package.github }})

{% endfor %}
