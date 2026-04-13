---
layout: default
title: Annotation Effort Type
---

## Annotation Type

### Power - Synthetic

{% assign power_synthetic = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Synthetic" %}

{% if power_synthetic.size > 0 %}
{% for item in power_synthetic %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Anonymized

{% assign power_anonymized = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Anonymized" %}

{% if power_anonymized.size > 0 %}
{% for item in power_anonymized %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Power - Compiled/Curated

{% assign power_compilation = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Curated" %}

{% if power_compilation.size > 0 %}
{% for item in power_compilation %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Power - Annotated

{% assign power_human = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Annotated" %}

{% if power_human.size > 0 %}
{% for item in power_human %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Synthetic

{% assign elec_synthetic = site.data.datasets
  | where: "domain", "Electronics"
  | where: "annotation_type", "Synthetic" %}

{% if elec_synthetic.size > 0 %}
{% for item in elec_synthetic %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Anonymized

{% assign elec_anonymized = site.data.datasets
  | where: "domain", "Electronics"
  | where: "annotation_type", "Anonymized" %}

{% if elec_anonymized.size > 0 %}
{% for item in elec_anonymized %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Electronics - Compiled/Curated

{% assign elec_compilation = site.data.datasets
  | where: "domain", "Electronics"
  | where: "annotation_type", "Curated" %}

{% if elec_compilation.size > 0 %}
{% for item in elec_compilation %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Electronics - Annotated

{% assign elec_human = site.data.datasets
  | where: "domain", "Electronics"
  | where: "annotation_type", "Annotated" %}

{% if elec_human.size > 0 %}
{% for item in elec_human %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Synthetic

{% assign built_synthetic = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "annotation_type", "Synthetic" %}

{% if built_synthetic.size > 0 %}
{% for item in built_synthetic %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Anonymized

{% assign built_anonymized = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "annotation_type", "Anonymized" %}

{% if built_anonymized.size > 0 %}
{% for item in built_anonymized %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}

### Built Environment - Compiled/Curated

{% assign built_compilation = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "annotation_type", "Curated" %}

{% if built_compilation.size > 0 %}
{% for item in built_compilation %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}


### Built Environment - Annotated

{% assign built_human = site.data.datasets
  | where: "domain", "Built Environment"
  | where: "annotation_type", "Annotated" %}

{% if built_human.size > 0 %}
{% for item in built_human %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% else %}
No matching datasets
{% endif %}
