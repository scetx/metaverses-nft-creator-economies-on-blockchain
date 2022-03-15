---
layout: blank
title: "Syllabus - Metaverses, NFTs..."
permalink: /syllabus
---

<table style="table-layout: fixed; font-size: 88%;">
  <thead>
      <th style="width: 10%;">Date</th>
      <th style="width: 45%;">Topic</th>
      <th style="width: 45%;">Assignments</th>
  </thead>
  <tbody>
    {% for row in site.data.syllabus %}
      <tr>
        <td style="text-align: center;">
          {{row.date}}
        </td>
        <td>
          {% if row.agenda.title %}
            <p style="margin: 0;">{{row.agenda.title}}</p>
          {% else %}
            <p>TBD</p>
          {% endif %}
          {% if row.agenda.recording %}
            [<a target="_blank" href="{{row.agenda.recording}}" style="font-size: 80%;text-decoration: underline;">Recording*</a>]
          {% endif %}
        </td>
        <td>
          {% for item in row.homework %}
            <li><a href="{{item.i.link}}" target="_blank">{{item.i.title}}</a></li>
          {% endfor %}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
