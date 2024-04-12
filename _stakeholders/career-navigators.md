---
layout: stakeholder
title: LER Ecosystem Map - Career Navigators
---
{% for item in site.data.stakeholders-list.stakeholders %}
	{% if item.name == "Career Navigators" %}
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



<div class="row section-bullet">

	{% for section in item.sections %}
		<div class="col-sm-5 body-text-medium section-bullet-text">
			<h3>{{ section.title }}</h3>
			{% for bullet in section.bullets %}

				{{ bullet }}

			{% endfor %}
		</div>
	{% endfor %}
</div>

{% endif %}
{% endfor %}





