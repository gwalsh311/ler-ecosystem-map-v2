---
layout: default
title: LER Ecosystem Map - Resources
---

<div class="container-fluid">

	<h2 class="sub-heading imagine">Resources</h2>
	
	{% for item in site.data.resources-list.resources %}

		<ul role="list">
				<li><a href="{{ item.url }}" target="_blank">{{ item.title }} {% if item.author %} - {{ item.author }}{% endif %}</a></li>
		</ul>

	{% endfor %}
</div>