---
layout: stakeholder
title: LER Ecosystem Map - Career Navigators
---
{% for item in site.data.stakeholders-list.stakeholders %}
{% if item.name == "Career Navigators" %}
<div class="row">
<div class="col-sm-2">
<img class="w-100" src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/>
</div>
<div class="col-sm-8">
<h1>{{ item.name }}</h1>
<div class="body-text-medium">
<p><strong>Definition: </strong>{{ item.definition }}</p>
<p><strong>Examples: </strong>{{ item.examples }}</p>
</div>
</div>
<div class="col-sm-2">
</div>
</div>
<div class="row">
<div class="col">
</div>
</div>
{% for section in item.sections %}
<div class="row">
<div class="col-sm-6 body-text-medium">
<h3>{{ section.title }}</h3>
<h4>{{ section.subheader}}</h4>
{% for bullet in section.bullets %}
<ul role="list">
<li>{{ bullet }}</li>
</ul>
{% endfor %}
</div>
</div>
{% endfor %}
{% endif %}
{% endfor %}





