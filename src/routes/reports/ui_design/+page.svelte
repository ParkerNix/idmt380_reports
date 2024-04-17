<script lang="ts">
	import Challenges from '$lib/assets/Challenges.png';
	import Cluster from '$lib/assets/Cluster.png';
	import Interview from '$lib/assets/Screenshot 2024-04-10 001543.png';
	import Notes from '$lib/assets/Screenshot 2024-04-10 122059.png';
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
						<strong>Prompt:</strong> "Design a responsive website for a funding company called 'Fundi'.
						The site's tone should be inspiring and professional and have home, product, and contact
						pages."
					</li>
					<li>
						<strong>Outcome:</strong>
						<ul>
							<li>Did what was asked in the prompt and provides responsive screens</li>
							<li>Content is arranged in a way that makes sense</li>
							<li>Design isn't the most visually appealing</li>
							<li>Does provide somewhat convincing copy text</li>
							<li>Not a big fan of the font choices</li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<strong>User Interview:</strong> For the user interview, my effectiveness definition was
				reliant on if the questions produced seemed helpful towards figuring out what the user
				really wants and needs. This tool did require a bit more manual input since it is a form and
				not a simple selection like the affinity mapping tool, but it did give a full script with
				valuable questions. The script includes an introduction paragraph to read before the
				questions, which lets the interviewee know there are no wrong answers, the purpose is to
				gather data, and that they may be recorded for team reference. Then, it has each of the
				entered topics with a list of questions underneath. The questions are pretty
				thought-provoking and open ended. For instance one question under the "Price" section asks,
				"How important is the price of food when you are choosing where to eat?" Questions like this
				do lead to great insights for a UX team to empathize with and understand the user.
				<strong>Effectiveness: 9/10</strong>
			</li>
			<hr />
			<li>
				<strong>"How Might We" Ideation:</strong> This tool's effectiveness was rated based off of
				whether or not the solutions it created answered the "How Might We" statement in a way that
				was reasonable and achievable. For the results I got, I found that many of the solutions
				were logically possible and did answer the statement. One suggestion was "Implement a mobile
				ordering system that allows users to pre-order their food and pick it up at a designated
				time," which was ultimately the solution our team ended up taking and found to be
				successful. Another solution said "Create a designated seating area for users who want to
				eat their food on the go, with convenient tables and chairs." While that would be nice for
				customers, The likelihood that the business we were working with, a small food truck, would
				ever be able to provide that is extremely low. This does show that the A.I. is not able to
				carry over information between tools, as it being a small business was mentioned in other
				parts of the test. This tool is certainly useful, but does have some issues and requires the
				user to be vigilant still.
				<strong>Effectiveness: 6/10</strong>
			</li>
		</ol>
	</div>
	<div class="section-card">
		<h2>Conclusion</h2>
		<p>
			In the end, I found QoQo to be a mixed bag; some tools were effective, and gave the user very
			helpful starting points from which they could ideate over. However, some tools either did not
			really do what they were meant to do as a result of faulty judgement or made poor suggestions
			due to a lack of persisting knowledge. I do feel as though tools like QoQo are immensely
			helpful for the average UX researcher and designer, so long as they are prepared to do some
			proofreading. It is definitely not anywhere near ready to take over jobs or anything, but some
			polish could definitely make it a strong ally.
		</p>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Gallery</h2>
		<div class="section-imgcard">
			<img src={Cluster} alt="QoQo's output for a Journey Map" />
			<img src={Challenges} alt="QoQo's output for a User Interview Script" />
			<img src={Interview} alt="QoQo's output for a How Might We statement and some solutions" />
			<img src={Notes} alt="Sticky notes from my food truck project" />
		</div>
	</div>
</div>
