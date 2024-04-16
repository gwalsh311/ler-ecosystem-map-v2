---
layout: default
title: LER Ecosystem Map - Resources
---
<div class="container-lg body-text-medium">
<div class="row">
<div class="col">
<h1>Resources</h1>
<div class="body-text-medium">
<p>A number of resources exist to help you learn more.</p>
</div>
</div>
</div>	
<div class="row"> 
<div class="col">
{% for item in site.data.resources-list.resources %}
<h2>{{ item.name }}</h2>
{% for site in item.sites %}
<ul>
<li><a href="{{ site.url }}" target="_blank">{{ site.title }}</a> | {{ site.author }}</li>
</ul>
{% endfor %}
{% endfor %}
</div>
</div>