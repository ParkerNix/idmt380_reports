<script lang="ts">
	import Framer1 from '$lib/assets/UI/Framer1.png';
	import Framer2 from '$lib/assets/UI/Framer2.png';
	import Framer3 from '$lib/assets/UI/Framer3.png';
	import Merrigo1 from '$lib/assets/UI/Merrigo1.png';
	import Merrigo2 from '$lib/assets/UI/Merrigo2.png';
</script>

<h1>Framer AI and Responsive Design</h1>
<div class="section">
	<div class="section-card">
		<h2>Research Goal</h2>
		<p>
			In this report, I will be looking at how the Framer AI handles responsive designs and if it
			can effectively generate them. This, of course, means I want to see how well it can generate
			designs with different screen sizes. Examining this tool will help to see where current AI is
			with being able to do what designers might find to be a tedious but necessary task.
		</p>
	</div>
	<div class="section-card">
		<h2>Tool Researched</h2>
		<p>
			My research will Framer, a design platform that allows users to create web designs, much like
			figma, and then easily deploy them. They explicitly state their ease of use and quick process
			from design to deployment. That being said, I am focusing on the AI portion of their design
			tool, which is meant to help you generate responsive designs via a short prompt.
		</p>
	</div>
	<div class="section-card">
		<h2>Implementation and Testing</h2>
		<p>To examine this tool, I followed these steps per test:</p>
		<ol>
			<li>
				<strong>Give Framer AI a prompt</strong> with details on tone and what should be included.
			</li>
			<li>
				<strong>Hit “Generate”</strong> and let the AI work
			</li>
			<li>
				<strong>Evaluate the resulting designs</strong> based on if they are designed for smaller screens
			</li>
			<li>
				<strong>Evaluate the general quality</strong> of the design
			</li>
		</ol>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Evaluation</h2>
		<p>
			To evaluate the effectiveness of each part of my testing, I give a few points on my thoughts
			about how the test went. Then, I take what I've found from each of the tests and try to pull
			some overall insights from the results.
		</p>
		<ol>
			<li>
				<ul>
					<li>
						<strong>Prompt:</strong> "Design a mobile-first app called "Wego". The site's tone should
						be cute and fun and have pages for planning trips, finding places to go, and adding friends."
					</li>
					<li>
						<strong>Outcome:</strong>
						<ul>
							<li>
								Calling it an app as opposed to a website didn't seem to make a big difference
							</li>
							<li>Was expecting the pages to be in separate frames, not on one long page</li>
							<li>The copy text is still pretty convincing</li>
							<li>
								Seems to have an interesting motif with emojis, but the font and monochrome pictures
								don't say “Cute and fun” to me
							</li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<ul>
					<li>
						<strong>Prompt:</strong> "Design a responsive website called “Merrigo”. The site's tone should
						be bright and elegant, with separate pages for finding bus tickets, purchasing tickets, and
						seeing purchased tickets."
					</li>
					<li>
						<strong>Outcome:</strong>
						<ul>
							<li>The design does not fit “Bright and Elegant”</li>
							<li>
								Some hand-drawn icons around the page block some pieces of text, also don't have
								good color contrast
							</li>
							<li>The font choice has been the best out of the three different prompts thus far</li>
							<li>
								Added in content that wasn't asked for, but didn't create the pages that were in the
								request
							</li>
							<li>Seems to always generate one page in desktop, tablet, and mobile-sized frame</li>
						</ul>
					</li>
				</ul>
			</li>
		</ol>
		<p>
			At this point, I had come to a conclusion about the responsive designs, but I wanted to also
			try seeing if I could get the AI to make a different kind of page, that being a store-like
			listing of bus tickets. These are the prompts I used:
		</p>
		<ol>
			<li>
				<ul>
					<li>
						<strong>Prompt:</strong> "A site called “Merrigo” for booking bus tickets. The site's tone
						should be bright and elegant and allow the user to find bus tickets in a list view."
					</li>
					<li>
						<strong>Outcome:</strong>
						<ul>
							<li>
								It is becoming obvious that the AI has a very specific pattern in mind for designing
								pages; All pages have a similar “generic homepage” feel to them, with a large hero
								at the top, some details about the product under that, and then some FAQs and/or a
								contact us section
							</li>
							<li>
								The AI did not generate a list view at all, and did not give the user the ability to
								find bus tickets in any capacity
							</li>
							<li>
								The colors for this were much brighter, but it was a rather aggressive orange this
								time and still had the monochrome pictures. In addition, the font choice was still
								off
							</li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<ul>
					<li>
						<strong>Prompt:</strong> "A page for booking bus tickets. This page should have a bright
						and elegant tone and should let the user find bus tickets in a grid with the price, time,
						and destination of the bus."
					</li>
					<li>
						<strong>Outcome:</strong>
						<ul>
							<li>
								Still did not do what was requested in the prompt and the user can't do any shopping
								for bus tickets
							</li>
							<li>
								Color scheme is still rather aggressive with a very bright and saturated coral color
							</li>
							<li>Font choice is still not fitting with the theme</li>
							<li>
								Definitely seems to have a set group of assets to pull from in terms of images; uses
								the Humaaans art style
							</li>
							<li>
								Does overall do a good job of moving content around so it fits on smaller screens,
								but it also has done a very similar layout the past few tries
							</li>
						</ul>
					</li>
				</ul>
			</li>
		</ol>
	</div>
	<div class="section-card">
		<h2>Conclusion</h2>
		<p>
			In the end, I found that the AI is capable of creating responsive designs. However, it is
			limited to one type of page, that being a homepage with some general information like product
			details and prices, FAQs, and contact information. This means that if you ask the AI to do
			anything outside of that, it will not be able to follow the prompts. In addition, it seems
			like its ability to create themes based off of some adjective combinations is lacking (as
			shown by the inconsistent theming with the adjectives "Bright and elegant" being given).
			Therefore, in terms of responsive design, I'd say it get a 9/10 for organizing and arranging
			properly, losing a point for generic design patterns. If I were to rate the tool for designing
			though, it would definitely be lower, probably around a 5/10 for how inconsistent it is with
			it's ability to follow prompts and derive theming from adjectives.
		</p>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Gallery</h2>
		<div class="section-imgcard">
			<img src={Framer1} alt="The resulting design for the first test" />
			<img src={Framer2} alt="The resulting design for the second test" />
			<img src={Framer3} alt="The resulting design for the third test" />
			<img src={Merrigo1} alt="The resulting design for the first Merrigo test" />
			<img src={Merrigo2} alt="The resulting design for the second Merrigo test" />
		</div>
	</div>
</div>
