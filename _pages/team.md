---
title: "Materials Modelling - Team"
layout: gridlay
excerpt: "Materials Modelling: Team members"
sitemap: false
permalink: /team/
---

## Principal Investigator


{% assign number_printed = 0 %}
{% for member in site.data.group_lead %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <br>
  <h4>{{ member.name }}</h4>
  <i>{{ member.info1 }}<br>{{ member.info2 }}<br>{{ member.info3 }}<br>email: {{ member.email | encode_email }}</i>
    
  {% if member.number_educ == 0 %}
  {% endif %}
    
  {% if member.number_educ == 1 %}
   {{ member.education1 }} 
  {% endif %}

  {% if member.number_educ == 2 %}
    {{ member.education1 }}
    {{ member.education2 }}
  {% endif %}

  {% if member.number_educ == 3 %}
    {{ member.education1 }} 
    {{ member.education2 }}
    {{ member.education3 }} 
  {% endif %}

  {% if member.number_educ == 4 %}
   {{ member.education1 }} 
   {{ member.education2 }} 
   {{ member.education3 }}
   {{ member.education4 }} 
  {% endif %}

  {% if member.number_educ == 5 %}
   {{ member.education1 }} 
   {{ member.education2 }} 
   {{ member.education3 }} 
   {{ member.education4 }} 
   {{ member.education5 }} 
  {% endif %}

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

<br>
<br>

## Group Members

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-5 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: {{ member.email | encode_email }}
</i> 
  <br> Topic: {{ member.topic }}
 
      {% if member.number_educ == 0 %}
    {% endif %}
  {% if member.number_educ == 1 %}
   {{ member.education1 }}
  {% endif %}

  {% if member.number_educ == 2 %}
   {{ member.education1 }} 
   {{ member.education2 }} 
  {% endif %}

  {% if member.number_educ == 3 %}
   {{ member.education1 }} 
   {{ member.education2 }} 
   {{ member.education3 }} 
  {% endif %}

  {% if member.number_educ == 4 %}
   {{ member.education1 }}
   {{ member.education2 }}
   {{ member.education3 }}
   {{ member.education4 }}
  {% endif %}

  {% if member.number_educ == 5 %}
   {{ member.education1 }}
   {{ member.education2 }}
   {{ member.education3 }}
   {{ member.education4 }}
   {{ member.education5 }}
  {% endif %}

</div>
  
<div class="col-sm-1 clearfix">  
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

## Alumni

### PhD

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members_phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-5 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br>  {{ member.current }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>
<div class="col-sm-1 clearfix">  
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

### MTech


{% assign number_printed = 0 %}
{% for member in site.data.alumni_members_mtech %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-5 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br>  {{ member.current }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>
<div class="col-sm-1 clearfix">  
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


### BS-MS


{% assign number_printed = 0 %}
{% for member in site.data.alumni_members_bs_ms %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-5 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br>  {{ member.current }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>
<div class="col-sm-1 clearfix">  
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

### PA/RA/Interns


<div class="row">

<div class="col-sm-5 clearfix">
<h4>Research/Project Assistants</h4>
{% for member in site.data.alumni_pa_ra_interns %}
{{ member.name }}
{% endfor %}
</div>
  
<div class="col-sm-1 clearfix">  
  </div>
  
<div class="col-sm-5 clearfix">
<h4>Interns</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
{% endfor %}
</div>
  
<div class="col-sm-1 clearfix">  
 </div>


</div>
