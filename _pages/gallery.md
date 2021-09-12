---
title: "Materials Modelling Group - Gallery"
layout: piclay
excerpt: "Materials Modelling Group -- Gallery"
permalink: /gallery/
---

# Gallery

{% assign number_printed = 0 %}
{% for pic in site.data.pictures_IISc %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
  
<---
<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>
-->

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

<p align="center">
  <img src="/images/picpic/image1.png" width="45%" />
  <img src="/images/picpic/sumeet-kiran.JPG" width="45%" /> 
</p>



<!---
![33rd annual symposium](/images/picpic/image1.png "Kiran receiving the certificate") ![33rd annual symposium](/images/picpic/sumeet-kiran.JPG "Sumeet and Kiran") 

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/image1.png" width="40%" >
</figure>

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/sumeet-kiran.JPG" width="40%" >
</figure>
-->
