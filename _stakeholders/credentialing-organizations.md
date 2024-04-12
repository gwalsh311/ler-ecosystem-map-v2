---
layout: stakeholder
title: LER Ecosystem Map - Credentialing Organizations
---
{% for item in site.data.stakeholders-list.stakeholders %}
{% if item.name == "Credentialing Organizations" %}
<div class="row">
<div class="col-sm-2">
<img class="w-100" src="../images/{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/>
</div>
<div class="col-sm-8">
<h1>{{ item.name }}</h1>
<div class="body-text-medium">
<p><strong>Definition: </strong>{{ item.definition }}</p>
<p><strong>Examples: </strong>{{ item.examples }}</p>
</div>
</div>
</div>

<div class="row">
<div class="col">
<div class="div-block-11"></div>
</div>
</div>
<div class="row">
<div class="col-sm-9">
<h1>Roles and Workstreams</h1>
<div class="row">
{% for section in item.sections %}
<div class="col-sm-6 body-text-medium">
<h3>{{ section.title }}</h3>
{% for bullet in section.bullets %}
<ul role="list">
<li>{{ bullet }}</li>
</ul>
{% endfor %}
</div>
{% endfor %}
</div>
<div class="row">
<div class="col">
<div class="div-block-11"></div>
</div>
</div>
{% include action-areas-intro.html %}
{% if item.action-areas and item.action-areas != '' %}
{% for item in item.action-areas %}
{% for action in site.data.action-items-content.actions %}
{% if action.name == item %}
<div class="row body-text-medium">
<div class="col">
<h3>{{ action.title }}</h3>
<p><strong>{{ action.description }}<br/></strong></p>
{% for item in action.bullets %}
<ul role="list">
<li>{{ item }}</li>
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
<div class="col body-text-medium">
{% for quote in item.quotes %}
<blockquote>{{ quote.text }} <div class="quote-description">&mdash; {{ quote.description }}</div></blockquote>
{% endfor %}
</div>
</div>

<div class="row business-case body-text-medium border">
<div class="col">
<h3>Business Case</h3>
<ul>
{% for case in item.business-case %}
<li><strong>{{ case.title }}</strong> - {{ case.description }}</li>
{% endfor %}
</ul>
</div>
</div>
<div class="row business-case body-text-medium">
<div class="col">
<h3>Social Case</h3>
<ul>
{% for case in item.social-case %}
<li><strong>{{ case.title }}</strong> - {{ case.description }}</li>
{% endfor %}
</ul>
</div>
</div>
</div>
{% endif %}
{% endfor %}