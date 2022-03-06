---
layout: blank
title: "Syllabus - Metaverses, NFTs..."
permalink: /syllabus
---

<table style="table-layout: fixed; font-size: 88%;">
  <thead>
      <th style="width: 10%;">Date</th>
      <th style="width: 45%;">Topic(s)</th>
      <th style="width: 45%;">Readings</th>
  </thead>
  <tbody>
    {% for row in site.data.syllabus %}
    <tr>
      <td style="text-align: center;"> 
        {{row.date}}
      </td>
      <td> 
        {% for item in row.agenda %}
        <li>{{item.i}}</li>
        {% endfor %}
      </td>
      <td>
        {% for item in row.readings %}
        <li><a href="{{item.i.link}}">{{item.i.title}}</a></li>
        {% endfor %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
