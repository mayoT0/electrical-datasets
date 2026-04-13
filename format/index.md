---
layout: default
title: Data Format
---

## Data Format and Structure

This page lists datasets by domain and dataset format and structure, showing the dataset title and URL.
For each domain, datasets are organized in the following format and structure order.

- Dataset
  - Domain: Power
    - Data Format and Structure:
      1. [Image-based](#power---image-based)
      2. [Structured](#power---structured)
      3. [Executable](#power---executable)
  - Domain: Electronics
    - Data Format and Structure:
      1. [Image-based](#electronics---image-based)
      2. [Structured](#electronics---structured)
      3. [Executable](#electronics---executable)
  - Domain: Built Environment
    - Data Format and Structure:
      1. [Image-based](#built-environment---image-based)
      2. [Structured](#built-environment---structured)
      3. [Executable](#built-environment---executable)

### Power - Image-based

{% assign power_image = site.data.datasets
  | where: "domain", "Power"
  | where: data_format, "Image-based" %}

{% if power_image.size > 0 %}
{% for item in power_image %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Structured

{% assign power_struct = site.data.datasets
  | where: "domain", "Power"
  | where: data_format, "Structured" %}

{% if power_struct.size > 0 %}
{% for item in power_struct %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Power - Executable

{% assign power_exec = site.data.datasets
  | where: "domain", "Power"
  | where: data_format, "Executable" %}

{% if power_exec.size > 0 %}
{% for item in power_exec %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Image-based

{% assign elec_image = site.data.datasets
  | where: "domain", "Electronics"
  | where: data_format, "Image-based" %}

{% if elec_image.size > 0 %}
{% for item in elec_image %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Structured

{% assign elec_struct = site.data.datasets
  | where: "domain", "Electronics"
  | where: data_format, "Structured" %}

{% if elec_struct.size > 0 %}
{% for item in elec_struct %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Executable

{% assign elec_exec = site.data.datasets
  | where: "domain", "Electronics"
  | where: data_format, "Executable" %}

{% if elec_exec.size > 0 %}
{% for item in elec_exec %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Image-based

{% assign built_image = site.data.datasets
  | where: "domain", "Built Environment"
  | where: data_format, "Image-based" %}

{% if built_image.size > 0 %}
{% for item in built_image %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Structured

{% assign built_struct = site.data.datasets
  | where: "domain", "Built Environment"
  | where: data_format, "Structured" %}

{% if built_struct.size > 0 %}
{% for item in built_struct %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Executable

{% assign built_exec = site.data.datasets
  | where: "domain", "Built Environment"
  | where: data_format, "Executable" %}

{% if built_exec.size > 0 %}
{% for item in built_exec %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}
