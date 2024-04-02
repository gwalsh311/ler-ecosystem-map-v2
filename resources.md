---
layout: default
title: LER Ecosystem Map - Resources
---
<div class="container-fluid">
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
		
		<ul role="list">
				<li><a href="{{ item.url }}" target="_blank">{{ item.title }} {% if item.author %} - {{ item.author }}{% endif %}</a></li>
		</ul>

	{% endfor %}
		</div>
	</div>
</div>