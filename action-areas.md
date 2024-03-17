---
layout: default
title: LER Ecosystem Map - Action Areas
---
<div class="container-fluid">
	<h2 class="sub-heading imagine">Action Areas</h2>

	<div class="body-text-small">Over the next 12-36 months, there are four key action areas that we believe LER ecosystem stakeholders should focus on to make significant progress towards adoption in service of equity and opportunity.
	</div>

	{% for action in site.data.action-items-content.actions %}

		<div class="row border">
			<div class="col">
				<h3 class="sub-heading map-copy">{{ action.title }}</h3>

				<p><strong>{{ action.description }}<br/></strong></p>

				{% for item in action.bullets %}

					<ul role="list">
						<li>{{ item }}</li>
					</ul>

				{% endfor %}
			</div>

			<div class="col">
				<div class="container-fluid">
					<div class="row text-center">

						{% for item in site.data.stakeholders-list.stakeholders %}

							{% if item.action-areas contains action.name %}
						
								<div class="col-sm-4 border text-center">

									<div><a class="dropdown-item" href="{{ site.baseurl }}{{ item.url }}"><img src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>

								</div> 
							{% endif %}	

						{% endfor %}

					</div>
				</div>
			</div>
		</div>
	{% endfor %}
</div>

