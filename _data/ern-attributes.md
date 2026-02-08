---
title: ERN Attribute Definition
layout: page
sidebar: main
permalink: /ern-attributes
---

This page lists the attribute definitions used in the Research Notebooks project.

## Attribute list

{% for row in site.data.ERNAttributeDefinition %}
- **{{ row.name }}**: {{ row.description }}
{% endfor %}
