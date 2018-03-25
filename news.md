---
layout: default
permalink: /news
title: News
---

# News
All the news about government financial transparency

<table>
    {% for name in site.data.news %}
      <tr>
            <td class="tablecolumn largetablecolumn">{{ name.date | date: '%B %d, %Y' }}</td>
            <td><a target="_blank" href="{{ name.source }}">{{ name.title }}</a></td>
      <tr>
            <td class="tablecolumn largetablecolumn">{{ name.author }}</td>
            <td>{{ name.excerpt }}</td>
      </tr>
      <tr><td colspan="2"><hr></td></tr>
    {% endfor %}

