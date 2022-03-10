---
layout: blank
title: "Syllabus - Metaverses, NFTs..."
permalink: /syllabus
---

<table style="table-layout: fixed; font-size: 88%;">
  <thead>
      <th style="width: 10%;">Date</th>
      <th style="width: 45%;">Topic(s)</th>
      <th style="width: 45%;">Assignments</th>
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
          {% else %}
            <li>TBD</li>
          {% endfor %}
        </td>
        <td>
          {% for item in row.homework %}
            <li><a href="{{item.i.link}}" target="_blank">{{item.i.title}}</a></li>
          {% else %}
            <li>None</li>
          {% endfor %}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
