---
layout: default
title: LER Ecosystem Map - Resources
---
<div class="container-lg body-text-medium">
<div class="row px-3 py-0">
<div class="col">
<h1>Resources</h1>
<div class="body-text-medium">
<p>A number of resources exist to help you learn more.</p>
</div>
</div>
</div>	
<div class="row px-3 py-0"> 
<div class="col">
{% for item in site.data.resources-list.resources %}
<h3>{{ item.name }}</h3>
{% for site in item.sites %}
<ul>
<li><a href="{{ site.url }}" target="_blank">{{ site.title }}</a> | {{ site.author }}</li>
</ul>
{% endfor %}
{% endfor %}
</div>
</div>