---
layout: default
title: Objective
---

## Objective

This page lists datasets by domain and dataset objective, showing the dataset title and URL.
For each domain, datasets are organized in the following objective order.

- Dataset
  - Domain: Power
    - Objective:
      1. [Computer Vision Task](#power---computer-vision-task)
      2. [Error Checking](#power---error-checking)
      3. [System Analysis](#power---system-analysis)
      4. [Decision Making](#power---decision)
  - Domain: Electronics
    - Objective:
      1. [Computer Vision Task](#electronics---computer-vision-task)
      2. [Error Checking](#electronics---error-checking)
      3. [System Analysis](#electronics---system-analysis)
      4. [Decision Making](#electronics---decision)
  - Domain: Built Environment
    - Objective:
      1. [Computer Vision Task](#built-environment---computer-vision-task)
      2. [Error Checking](#built-environment---error-checking)
      3. [System Analysis](#built-environment---system-analysis)
      4. [Decision Making](#built-environment---decision)

### Power - Computer Vision Task

{% assign power_cv = site.data.datasets
  | where: "domain", "Power"
  | where: "objective", "Computer Vision Task" %}

{% if power_cv.size > 0 %}
{% for item in power_cv %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Error Checking

{% assign power_checking = site.data.datasets
  | where: "domain", "Power"
  | where: "objective", "Error Checking" %}

{% if power_checking.size > 0 %}
{% for item in power_checking %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Power - System Analysis

{% assign power_analysis = site.data.datasets
  | where: "domain", "Power"
  | where: "objective", "System Analysis" %}

{% if power_analysis.size > 0 %}
{% for item in power_analysis %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Decision Making

{% assign power_decision = site.data.datasets
  | where: "domain", "Power"
  | where: "objective", "Decision Making" %}

{% if power_decision.size > 0 %}
{% for item in power_decision %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Computer Vision Task

{% assign elec_cv = site.data.datasets
  | where: "domain", "Electronics"
  | where: "objective", "Computer Vision Task" %}

{% if elec_cv.size > 0 %}
{% for item in elec_cv %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Error Checking

{% assign elec_checking = site.data.datasets
  | where: "domain", "Electronics"
  | where: "objective", "Error Checking" %}

{% if elec_checking.size > 0 %}
{% for item in elec_checking %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - System Analysis

{% assign elec_analysis = site.data.datasets
  | where: "domain", "Electronics"
  | where: "objective", "System Analysis" %}

{% if elec_analysis.size > 0 %}
{% for item in elec_analysis %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Decision Making

{% assign elec_decision = site.data.datasets
  | where: "domain", "Electronics"
  | where: "objective", "Decision Making" %}

{% if elec_decision.size > 0 %}
{% for item in elec_decision %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Computer Vision Task

{% assign built_cv = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "objective", "Computer Vision Task" %}

{% if built_cv.size > 0 %}
{% for item in built_cv %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Error Checking

{% assign built_checking = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "objective", "Error Checking" %}

{% if built_checking.size > 0 %}
{% for item in built_checking %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - System Analysis

{% assign built_analysis = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "objective", "System Analysis" %}

{% if built_analysis.size > 0 %}
{% for item in built_analysis %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Decision Making

{% assign built_decision = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "objective", "Decision Making" %}

{% if built_decision.size > 0 %}
{% for item in built_decision %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% else %}
No matching datasets
{% endif %}
