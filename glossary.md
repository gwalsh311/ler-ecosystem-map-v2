---
layout: default
title: LER Ecosystem Map - Glossary
---

<div class="container-fluid">

	<h2 class="sub-heading imagine">Glossary</h2>

	<p>These terms reference the draft glossary at the T3 Innovation Network Learning & Employment Record Guide.</p>
	
	{% for item in site.data.glossary-list.terms %}

		<div>
			<p><strong>{{ item.term }}</strong></p>
			<p>{{ item.definition }}</p>

		</div>

	{% endfor %}
</div>