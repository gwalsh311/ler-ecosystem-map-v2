---
layout: default
title: LER Ecosystem Map - Action Areas
---
<div class="container-fluid">
	<h2 class="sub-heading imagine">Action Areas</h2>

	<div class="body-text-small">Over the next 12-36 months, there are four key action areas that we believe LER ecosystem stakeholders should focus on to make significant progress towards adoption in service of equity and opportunity.
	</div>

<!-- Defining Value Propositions -->

	<div class="row border">
		<div class="col">
			<h3 class="sub-heading map-copy">Defining Value Propositions</h3>

			<p><strong>Include key stakeholder groups in the development of compelling value propositions that demonstrate the value of LERs.<br/></strong></p>

			<ul role="list">
				<li>Identify how using LERs is different from current practice, and how LER’s can help stakeholders advance their existing goals/agendas.</li>
			</ul>

			<ul role="list">
				<li>Consider variation within stakeholder groups (e.g. SMEs versus large corporations, post-secondary institutions vs professional certification providers).</li>
			</ul>

			<ul role="list">
				<li>Define metrics of success, test the messaging with stakeholders, and refine</li></ul><ul role="list"><li>Add data points to convert propositions into value statements</li></ul><ul role="list"><li>Use the process to build momentum and find champions for LERs — prioritize employers, learners, earners, and state governance.</li>
			</ul>

			<ul role="list">
				<li>Add data points to convert propositions into value statements.</li>
			</ul>

			<ul role="list">
				<li>Use the process to build momentum and find champions for LERs — prioritize employers, learners, earners, and state governance.</li>
			</ul>
		</div>
		<div class="col">
			<div class="container-fluid">
				<div class="row text-center">
					{% for item in site.data.stakeholders-list.stakeholders %}

						{% for area in item.action-areas %}

							{% if area == "defining" %}

								<div class="col-sm-4 border text-center">

									<div><a class="dropdown-item" href="{{ site.baseurl }}{{ item.url }}"><img src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>

								</div>

							{% endif %}

						{% endfor %}

					{% endfor %}

				</div>

			</div>

		</div>
	</div>
</div>

<!-- Building Employer Demand -->
<div class="container-fluid">
	<div class="row border">
		<div class="col">
			<h3 class="sub-heading map-copy">Building Employer Demand</h3>

			<p><strong>Strengthen employer demand and capacity for LERs.<br/></strong></p>

			<ul role="list">
				<li>Work with HR systems and ATS systems to increase support for integration of data from LERs.</li>
			</ul>

			<ul role="list">
				<li>Connect supply and demand by increasing the number of verifiable credentials issued by education providers, and supporting learners and earners in their use of LERs to apply for jobs and other opportunities.</li>
			</ul>

			<ul role="list">
				<li>Engage workforce development and other support systems, to widen the pipeline of skills-based talent.</li>
			</ul>

			<ul role="list">
				<li>Demonstrate the value of LERs in up/reskill pilots with current employees.</li>
			</ul>

			<ul role="list">
				<li>Pilot and scale the issuing of employment records to employees.</li>
			</ul>
		</div>
		<div class="col">

			<div class="container-fluid">
				<div class="row text-center">
					{% for item in site.data.stakeholders-list.stakeholders %}

						{% for area in item.action-areas %}

							{% if area == "building" %}

								<div class="col-sm-4 border">

									<div><a class="dropdown-item" href="{{ site.baseurl }}{{ item.url }}"><img src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>


								</div>

							{% endif %}

						{% endfor %}

					{% endfor %}

				</div>

			</div>

		</div>
	</div>
</div>


<!-- Gathering Data on Impact -->
<div class="container-fluid">
	<div class="row" border>
		<div class="col">
			<h3 class="sub-heading map-copy">Gathering Data on Impact</h3>

			<p><strong>Define success metrics and collect data on impact across all workstreams to answer the key question: How do we know it’s working?<br/></strong></p>

			<ul role="list">
				<li>Collect empirical data that proves out the value propositions for LERs, relevant to each stakeholder pain points or opportunities.</li>
			</ul>

			<ul role="list">
				<li>For learner and earner, this could include demonstrating how LERs can lead to great access to good jobs and other opportunities, considering the entire set of skills and abilities they have earned through education, work, and life experiences.</li>
			</ul>

			<ul role="list">
				<li>For employers, major impact metrics would demonstrate better access to a skilled talent pool, show reduced time to fill job roles, improved quality of candidates hired (i.e., better fit), and reduced cost to fill jobs, and ability to predict on-the-job success.</li>
			</ul>

			<ul role="list">
				<li>Overall, gather data to show how LERs assist in removing barriers to education and employment.</li>
			</ul>
		</div>
		<div class="col">
			<div class="container-fluid">
				<div class="row text-center">
					{% for item in site.data.stakeholders-list.stakeholders %}

						{% for area in item.action-areas %}

							{% if area == "gathering" %}

								<div class="col-sm-4 border">

									<div><a class="dropdown-item" href="{{ site.baseurl }}{{ item.url }}"><img src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>

								</div>

							{% endif %}

						{% endfor %}

					{% endfor %}

				</div>

			</div>

		</div>
	</div>
</div>

<!-- Shifting to a Skills-Based System -->
<div class="container-fluid">
	<div class="row border">
		<div class="col">
			<h3 class="sub-heading map-copy">Shifting to a Skills-Based System</h3>

			<p><strong>Make sure that the system we’re building supports skills-based hiring.<br/></strong></p>

			<ul role="list">
				<li>Holistically support transformation to a skills-based system of learning, earning and career discovery.</li>
			</ul>

			<ul role="list">
				<li>Offer skills-based language and education for all key stakeholders (including learners and earners, employers, HR systems, etc.).</li>
			</ul>

			<ul role="list">
				<li>Remove requirements for bachelor’s degrees where they are not needed.</li>
			</ul>

			<ul role="list">
				<li>Develop effective skills-based matching for open roles to help employers replace other ways to assess job-fit.</li>
			</ul>

			<ul role="list">
				<li>Expand data systems to enable states and other major stakeholders to link employment, credentials and skills data.</li>
			</ul>
			<ul role="list">
				<li>Build state-level competency models to inform LERs and job requirements.</li>
			</ul>
		</div>
		<div class="col">
			<div class="container-fluid">
				<div class="row text-center">
					{% for item in site.data.stakeholders-list.stakeholders %}

						{% for area in item.action-areas %}

							{% if area == "shifting" %}

								<div class="col-sm-4 border">

									<div><a class="dropdown-item" href="{{ site.baseurl }}{{ item.url }}"><img src="{{ item.icon }}" loading="lazy" alt="{{ item.icon-alt }}"/><br/>{{ item.name }}</a></div>

								</div>

							{% endif %}

						{% endfor %}

					{% endfor %}

				</div>

			</div>

		</div>
	</div>
</div>

