---
layout: stakeholder
title: LER Ecosystem Map - LER Solution Providers
---
{% for item in site.data.stakeholders-list.stakeholders %}
{% if item.name == "LER Technology Providers" %}
<div class="row mt-2">
<div class="col-sm-2">
<img class="w-100" src="../images/{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/>
</div>
<div class="col-sm-10">
<h1>{{ item.name }}</h1>
<p><strong>Definition: </strong>{{ item.definition }}</p>
<p><strong>Examples: </strong>{{ item.examples }}</p>
</div>
</div>



<div class="row">
<div class="col-sm-9">
<h1 class="aliceblue">Roles and Workstreams</h1>
<div class="row mx-1">
{% for section in item.sections %}
<div class="col-sm-6">
<h3>{{ section.title }}</h3>
{% for bullet in section.bullets %}
<ul role="list">
<li>{{ bullet }}</li>
</ul>
{% endfor %}
</div>
{% endfor %}
</div>


{% if item.action-areas and item.action-areas != '' %}
{% include action-areas-intro.html %}
{% for item in item.action-areas %}
{% for action in site.data.action-items-content.actions %}
{% if action.name == item.title %}
<div class="row mx-1">
<div class="col">
<h3>{{ action.title }}</h3>
<p>{{ action.description }}<br/></p>
{% for bullet in item.bullets %}
<ul role="list">
<li>{{ bullet }}</li>
</ul>
{% endfor %}
</div>
</div>
{% endif %}
{% endfor %}
{% endfor %}
{% endif %}
</div>

<div class="col-sm-3">

<div class="row">
<div class="col">
{% if item.quote-text %}
<blockquote>
<span class="quote">&ldquo;</span>{{ item.quote-text }}<span class="quote">&rdquo;</span> <div class="quote-description">&mdash; {{ item.quote-description }}</div></blockquote>
{% endif %}
</div>
</div>

<div class="row business-case">
<div class="col">
<h3>Business Case</h3>
{% for case in item.business-case %}
<p><strong>{{ case.title }}</strong> - {{ case.description }}</p>
{% endfor %}
</div>
</div>
<div class="row business-case">
<div class="col">
<h3>Social Case</h3>
{% for case in item.social-case %}
<p><strong>{{ case.title }}</strong> - {{ case.description }}</p>
{% endfor %}
</div>
</div>
</div>
{% endif %}
{% endfor %}