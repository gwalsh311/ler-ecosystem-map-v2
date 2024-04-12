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
<div class="col-sm-2">
</div>
</div>
{% include action-areas-intro.html %}
{% if item.action-areas and item.action-areas != '' %}
{% for item in item.action-areas %}
{% for action in site.data.action-items-content.actions %}
{% if action.name == item %}
<div class="row section-bullet body-text-small action-area">
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

<div class="row body-text-medium">
<div class="col-sm-2">
</div>
<div class="col-sm-4 business-case">
<h3>Business Case</h3>
<ul>
{% for case in item.business-case %}
<li><strong>{{ case.title }}</strong> - {{ case.description }}</li>
{% endfor %}
</ul>
</div>

<div class="col-sm-4 business-case">
<h3>Social Case </h3>
<ul>
{% for case in item.social-case %}
<li><strong>{{ case.title }}</strong> - {{ case.description }}</li>
{% endfor %}
</ul>
</div>
<div class="col-sm-2">
</div>
</div>

<div class="row">
<div class="col-sm-2">
</div>

<div class="row">
<div class="col-sm-3"></div>
<div class="col-sm-6 quote">
{% for quote in item.quote %}
<blockquote>{{ quote.title }}</blockquote>
<p>{{ quote.description}}</p>
{% endfor %}
</div>
<div class="col-sm-3"></div>
</div>

<div class="row section-bullet">

{% for section in item.sections %}
<div class="col-sm-5 body-text-medium section-bullet-text">
<h3>{{ section.title }}</h3>
<h4>{{ section.subheader}}</h4>
{% for bullet in section.bullets %}

{{ bullet }}

{% endfor %}

</div>

{% endfor %}
</div>

{% endif %}
{% endfor %}