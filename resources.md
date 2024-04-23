---
layout: default
title: LER Ecosystem Map - Resources
---
<div class="container-fluid">
    <div class="row mx-4 py-3">
    	<div class="col">
        	<h1>Resources</h1>
    	</div>
 	</div>
	<div class="row mx-4">
        <div class="col">
			<p>A number of resources exist to help you learn more.</p>
		</div>
	</div>	
	<div class="row mx-4">
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
</div>