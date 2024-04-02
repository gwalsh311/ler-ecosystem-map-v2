---
layout: default
title: LER Ecosystem Map - Action Areas
---
<div class="container-fluid section-intro">
<div class="row">
	<div class="col-sm-2">
		<img class="w-100" src="../images/{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/>
	</div>
	<div class="col-sm-8">
		<h1>Action Areas</h1>
			<div class="body-text-medium">
				<p>Over the next 12-36 months, there are four key action areas that we believe LER ecosystem stakeholders should focus on to make significant progress towards adoption in service of equity and opportunity.</p>
			
			</div>
	</div>
</div>	

	{% for action in site.data.action-items-content.actions %}

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

			<div class="col">
				<div class="container-fluid">
					<div class="row text-center">

						{% for item in site.data.stakeholders-list.stakeholders %}

							{% if item.action-areas contains action.name %}
						
								<div class="col-sm-4 text-center">

									<div><a class="dropdown-item" href="{{ site.baseurl }}/stakeholder/{{ item.url }}"><img src="./images/{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>

								</div> 
							{% endif %}	

						{% endfor %}

					</div>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="col-sm-12 action-spacer"></div>
		</div>
	{% endfor %}
</div>

