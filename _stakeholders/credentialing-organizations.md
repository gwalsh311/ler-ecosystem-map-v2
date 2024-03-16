---
layout: default
title: LER Ecosystem Map - Credentialing Organizations
---
{% for item in site.data.stakeholders-list.stakeholders %}
{% if item.name == "Credentialing Organizations" %}
<div class="row">
<div class="col-sm-2">
<img class="w-100" src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/>
</div>
<div class="col-sm-10">
<h1>{{ item.name }}</h1>
</div>
</div>
<div class="row">
<div class="col">
<p><strong>Definition: </strong>{{ item.definition }}</p>
<p><strong>Examples: </strong>{{ item.examples }}</p>
</div>
</div>
{% endif %}
{% endfor %}