---
layout: stakeholder
title: LER Ecosystem Map - LER Solution Providers
---
{% for item in site.data.stakeholders-list.stakeholders %}
{% if item.name == "LER Solution Providers" %}
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
<div class="row">
<div class="col">
<h3>Business Case</h3>
{% for case in item.business-case %}
<p><strong>{{ case.title }}</strong> - {{ case.description }}</p>
{% endfor %}
</div>
</div>
<div class="row">
<div class="col">
<h3>Social Case </h3>
{% for case in item.social-case %}
<p><strong>{{ case.title }}</strong> - {{ case.description }}</p>
{% endfor %}
</div>
</div>
{% for section in item.sections %}
<div class="row">
<div class="col">
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