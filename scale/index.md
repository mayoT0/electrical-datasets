---
layout: default
title: Dataset Scale
---

## Dataset Scale

This page lists datasets by domain and dataset scale, showing the dataset title and URL.
For each domain, datasets are organized in the following dataset scale order.

- Dataset
  - Domain: Power
    - Dataset Scale:
      1. [Small-scale/single-domian](#power---small)
      2. [Large-scale/benchmark](#power---large)
  - Domain: Electronics
    - Dataset Scale:
      1. [Small-scale/single-domian](#power---small)
      2. [Large-scale/benchmark](#power---large)
  - Domain: Built Environment
    - Dataset Scale:
      1. [Small-scale/single-domian](#power---small)
      2. [Large-scale/benchmark](#power---large)

### Power - Small

{% assign power_small = site.data.datasets
  | where: "domain", "Power"
  | where: "scale", "Small" %}

{% if power_small.size > 0 %}
{% for item in power_small %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Large

{% assign power_large = site.data.datasets
  | where: "domain", "Power"
  | where: "scale", "Large" %}

{% if power_large.size > 0 %}
{% for item in power_large %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Small

{% assign elec_small = site.data.datasets
  | where: "domain", "Electronics"
  | where: "scale", "Small" %}

{% if elec_small.size > 0 %}
{% for item in elec_small %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Large

{% assign elec_large = site.data.datasets
  | where: "domain", "Electronics"
  | where: "scale", "Large" %}

{% if elec_large.size > 0 %}
{% for item in elec_large %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Small

{% assign built_small = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "scale", "Small" %}

{% if built_small.size > 0 %}
{% for item in built_small %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Large

{% assign built_large = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "scale", "Large" %}

{% if built_large.size > 0 %}
{% for item in built_large %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}
