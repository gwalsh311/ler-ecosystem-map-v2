---
layout: default
title: LER Ecosystem Map - Glossary
---

<div class="container-fluid">
    <div class="row mx-4 py-3">
    	<div class="col">
        	<h1>Glossary</h1>
    	</div>
 	</div>
 	<div class="row mx-4">
        <div class="col">
			<p>These terms reference the draft glossary in progress with the T3 Innovation Network Learning & Employment Record Guide.</p>
		</div>
	</div>
	<div class="row mx-4">
		<div class="col">
			{% for item in site.data.glossary-list.terms %}
				<h3>{{ item.term }}</h3>
				{% if item.definition %}
					<p>{{ item.definition }}</p>
				{% endif %}
				{% if item.list %}
					<ol role="list">
						{% for option in item.list %}
							<li>{{ option }}</li>
						{% endfor %}
					</ol>
				{% endif %}
			{% endfor %}
		</div>
	</div>
</div>
