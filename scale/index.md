---
layout: default
title: Dataset Scale
---

# Dataset Directory

## Scale (Grouped by Domain)

{% assign domains = site.data.datasets | group_by: "domain" %}

{% for domain in domains %}
## {{ domain.name }}

{% assign small = domain.items | where: "scale", "Small" %}
{% assign large = domain.items | where: "scale", "Large" %}

{% if small.size > 0 %}
### Small scale

{% for item in small %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endif %}

{% if large.size > 0 %}
### Large scale

{% for item in large %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endif %}

{% endfor %}