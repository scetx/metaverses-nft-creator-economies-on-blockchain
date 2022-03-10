---
layout: blank
title: "Speakers - Metaverses, NFTs..."
permalink: /speakers
---

<table style="table-layout: fixed; font-size: 88%;">
  <thead>
      <th style="width: 40%;">Company(s)</th>
      <th style="width: 60%;">Speaker(s)</th>
  </thead>
  <tbody>
    {% for row in site.data.speakers %}
    <tr>
      <td> 
        {% if row.company %} 
          {{row.company}}
        {% else %}
          N/A
        {% endif %}
      </td>
      <td> 
        {% if row.speakers %} 
          {{row.speakers}}
        {% else %}
          TBD
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
