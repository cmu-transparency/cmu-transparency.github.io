---
title: "Accountable Systems Lab - Team"
layout: gridlay
excerpt: "Accountable Systems Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 <!-- **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** -->


<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/person/thumbs/{{member.photo}}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}>
  <br>website: <{{ member.website }}></i>
  <ul style="overflow: hidden">
  </ul>
 </div>
 {% assign number_printed = number_printed | plus: 1 %}

 {% if even_odd == 1 %}
 </div>
 {% endif %}

 {% endfor %}

 {% assign even_odd = number_printed | modulo: 2 %}
 {% if even_odd == 1 %}
 </div>
 {% endif %}






## Master and Bachelor Students


## Alumni
<!-- <table align="center" style="width:100%">
<tr>
    <th>Master Students</th>
    <th>Bachelor Students</th>
  </tr>
</table> -->
