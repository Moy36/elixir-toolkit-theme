---
title: ERN Attribute Definition
layout: page
sidebar: main
permalink: /ern-attributes
---

This page lists the attribute definitions used in the Research Notebooks project.

## Attribute Table

| ID | Attribute | Description |
|----|----------|-------------|
{% for row in site.data.ERNAttributeDefinition %}
| {{ row["ID"] }} | {{ row["Name of Attributes"] }} | {{ row["Description/expected content"] }} |
{% endfor %}
