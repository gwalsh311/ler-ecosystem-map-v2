---
layout: default
title: LER Ecosystem Map - LER Guidance
---

<div class="container-fluid">
    <div class="row mx-4 py-3">
    	<div class="col">
        	<h1>Technical Guidance</h1>
    	</div>
 	</div>
   	<div class="row mx-4">
    	<div class="col">
    		<p>LERs are digital credentials representing learning and employment related achievements. LERs may be both a single credential and a collection of credentials. In a lifetime, one may earn many LERs.</p>
    		<p>For LERs to be effective at scale, they must be able to function across a variety of systems online where individuals may seek to use their employment and education data. The recommended path to LER interoperability across the web is to leverage the web standard, <a href="https://www.w3.org/TR/vc-data-model/" target="_blank">W3C Verifiable Credentials</a>. Verifiable Credentials provides a container that may be used for LER achievement data and the instructions for how LERs could be digitally signed. Verifiers of LERs use software that checks the integrity of the digital signature and that the credential hasn’t been tampered with since it was issued. They may check additional data points such as whether the credential has been revoked or expired, if the issuer identity can be trusted, and if the content in the LER is suitable for the context in which it is being used.</p>
    		<p>As the Digital Credentials Consortium describes in their white paper, <a href="https://digitalcredentials.mit.edu/docs/DCC-Making-Sense-of-Key-Data-Standards-for-Verifiable-LERs.pdf" target="_blank">Making Sense of the Key Data Standards for Verifiable LERs</a>, the 1EdTech standards, <a href="https://www.imsglobal.org/spec/ob/v3p0" target="_blank">Open Badges 3.0</a> and <a href="https://www.imsglobal.org/spec/clr/v2p0" target="_blank">Comprehensive Learner 2.0 (CLR v2)</a>, function like W3C Verifiable Credentials. As with previous versions of these standards, the latest versions can accommodate rich descriptions of learning and employment. Unlike previous versions, Open Badges 3.0 and Comprehensive Learner Record 2.0 can be digitally signed, making them suitable for the issuance of formal documents such as degrees and transcripts.</p>
    		<p>Advantages of Verifiable Credentials:</p>
    		<ul role="list">
				<li>Issued on demand</li>
				<li>Digitally signed by issuer</li>
				<li>Can’t be changed once signed</li>
				<li>Identity provided by L/Earner
					<ul role="list">
						<li>Could be a decentralized id</li>
						<li>Could be other identity agreed upon with issuer</li>
						<li>Doesn’t need to be an email address which could be changed or lost</li>
					</ul>
				</li>
				<li>Stored in web or mobile wallets that l/earners control</li>
				<li>L/earner controls privacy
					<ul role="list">
						<li>Decides with whom or what to share</li>
						<li>Verification is between verifier and l/earner</li>
						<li>Issuer is not contacted for verification</li>
					</ul>
				</li>
			</ul>
			<p>It’s often asked if learning and employment records issued using older digital credentials standards, as PDFS, or other formats besides Verifiable Credentials are considered to be “LERs”. The answer is yes, but they will be inherently less usable on the web when Verifiable Credentials are expected. For as long as they are hosted by their issuing web platforms, Open Badges 2.0 and earlier should be available to share online but they will not be verifiable in the same cryptographic manner because they won’t be digitally signed. PDFs will likely continue to have their place in the world but even digitally signed PDFs are not as functionally usable as the machine readable data in Verifiable Credentials.</p>
		</div>
	</div>
    <div class="row">
    	<div class="col">
      		<div class="div-block-12"></div>
    	</div>
  	</div>
  	<div class="row mx-4">
  		<div>
			<p><a href ="https://www.c-ben.org/wp-content/uploads/2023/03/CBEN-23-003-Interoperable-Learning-WALMART-V2.pdf" target="_blank">The Competency Based Education Network Interoperability Principles </a> offer guidance and key design elements for optimal LER systems. Recognition and adherence to these principles is encouraged for technology vendors and other decision makers within the ecosystem.</p>
		<div>
			<p><strong>OPEN STANDARDS</strong></p>
			<p>Data included in LERs are formatted using a standard structure, allowing for easy exchange between individuals, education, and employment.</p>
		</div>
		<div>
			<p><strong>PRIVACY AND SECURITY</strong></p>
			<p>Systems protect the privacy and security of individuals' data, which, in turn, builds and maintains trust in LERs.</p>
		</div>
		<div>
			<p><strong>UNLOCKING LEARNING ANYWHERE</strong></p>
			<p>Learning is lifelong, and quality learning can occur outside of the classroom. Interoperable LERs honor the value of all learning and offer processes for validating a wide range of learning, skills, and competencies.</p>
		</div>
		<div>
			<p><strong>GLOBAL MOBILITY</strong></p>
			<p>Interoperable LERs support learners' mobility by functioning in local, regional, state, national, and global talent marketplaces.</p>
		</div>
		<div>
			<p><strong>UNIVERSAL ACCESS</strong></p>
			<p>Interoperable LERs are user-centered and ensure every potential user has access to and control over a digital wallet to store, manage, and curate LERs.</p>
		</div>
		<div>
			<p><strong>ALIGNMENT</strong></p>
			<p>All stakeholders, including employers, states, and local, regional and, federal agencies, are aligned, intentionally collaborating to support and ensure fidelity to interoperability principles.</p>
		</div>
		<div>
			<p><strong>PUBLIC AND PRIVATE PARTNERSHIPS CREATING PUBLIC GOOD</strong></p>
			<p>A healthy marketplace is cultivated and regulated to both encourage innovation and ensure that the benefits of interoperable LERs are shared by all stakeholders.</p>
		</div>
	</div>
</div>
