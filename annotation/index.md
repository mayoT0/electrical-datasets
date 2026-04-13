---
layout: default
title: Annotation Effort Type
---

# Dataset Directory

## Annotation Type

### Power - Synthetic


{% assign power_synthetic = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Synthetic" %}

{% for item in power_synthetic %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}


### Power - Anonymized


{% assign power_anonymized = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Anonymized" %}

{% for item in power_anonymized %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}


### Power - Compiled/Curated


{% assign power_compilation = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Curated" %}

| Title | Link |
| :---- | :--- |
{% for item in power_compilation %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}


### Power - Synthetic


{% assign power_human = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Annotated" %}

| Title | Link |
| :---- | :--- |
{% for item in power_human %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
