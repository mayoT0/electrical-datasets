---
layout: default
title: Dataset Directory
---

# Dataset Directory

---

## Format

{% assign by_format = site.data.datasets | group_by: "data_format" %}
{% for format in by_format %}
### {{ format.name }}

| Title | Link |
|------|------|
{% for item in format.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}

---

## Scale

{% assign by_scale = site.data.datasets | group_by: "scale" %}
{% for scale in by_scale %}
### {{ scale.name }}

| Title | Link |
|------|------|
{% for item in scale.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}

---

## Objective

{% assign by_objective = site.data.datasets | group_by: "objective" %}
{% for obj in by_objective %}
### {{ obj.name }}

| Title | Link |
|------|------|
{% for item in obj.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}

---

## Annotation Type

{% assign by_annotation = site.data.datasets | group_by: "annotation_type" %}
{% for ann in by_annotation %}
### {{ ann.name }}

| Title | Link |
|------|------|
{% for item in ann.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}