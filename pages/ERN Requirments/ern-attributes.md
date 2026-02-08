---
title: ERN Attribute Definition
layout: page
sidebar: main
permalink: /ern-attributes
---

This page lists the attribute definitions used in the Research Notebooks project.

## Attribute Table


<table class="ern-table">
  <colgroup>
    <col style="width: 15%;">
    <col style="width: 30%;">
    <col style="width: 55%;">
  </colgroup>

  {% for row in site.data.ERNAttributeDefinition %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
