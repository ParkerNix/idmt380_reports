<script lang="ts">
	import Challenges from '$lib/assets/Challenges.png';
	import Cluster from '$lib/assets/Cluster.png';
	import Interview from '$lib/assets/Screenshot 2024-04-10 001543.png';
	import Notes from '$lib/assets/Screenshot 2024-04-10 122059.png';
</script>

<h1>UX Design and QoQo</h1>
<div class="section">
	<div class="section-card">
		<h2>Research Goal</h2>
		<p>
			In this report, I will be looking to find how A.I. tools help UX designers accomplish their
			job more easily with current-day technology. I am mostly looking to find how these tools can
			help facilitate the tedious parts of UX Design, such as organizing notes, creating interview
			scripts, and so on. To do this, I will be looking at a specific tool, QoQo, to see if it is
			effective in organizing data, as well as ideating to find solutions and making things like
			scripts for the researcher to use in the field. In doing this, I will be able to analyze the
			results it gives me so that I can give a rating from 1 to 10 on how well it was able to
			complete it's task.
		</p>
	</div>
	<div class="section-card">
		<h2>Tool Researched</h2>
		<p>
			My research will focus on the tool, QoQo (pronounced "coco"), which is a plugin made to work
			with Figma. It was created with the intention to automate the process of creating user journey
			maps, generating affinity diagrams, writing interview scripts, an so on. This is a paid tool,
			so it is somewhat inconvenient for the average user. That being said, I do feel as though the
			potential for it to make researching and designing easier is very promising.
		</p>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Implementation and Testing</h2>
		<p>
			To test this tool, I took a project I worked on a few years back that had a focus on UX
			research and design. I then used the QoQo tool to do three things:
		</p>
		<ol>
			<li>
				<strong>Make an affinity map</strong> using notes taken from several user interviews and QoQo's
				"Affinity Mapping" tool. This tool allows you to either use a text transcript of a user interview
				or a group of sticky notes if you've already put your data into Figma. I chose to use the sticky
				notes I had from the project, which meant all I had to do was select all the sticky notes and
				hit "Cluster", which starts the grouping process. After a few seconds, it had finished grouping
				the items into three named groups.
			</li>
			<hr />
			<li>
				<strong>Make a interview script</strong> based off of some persona information and general interview
				topics with their "Use Interview" tool. This was more of a form where it asked you to input information
				like the age, gender, and occupation of a persona you are targeting, a general situation the
				user would be in that they would be interacting with your product, and some topics to ask questions
				about. After inputting all of that, it gave me a list of questions grouped by the different topics
				I had entered.
			</li>
			<hr />
			<li>
				<strong>Make a "How Might We" statement</strong> with potential solutions to solve the users
				issues with their "How Might We" tool. This tool only asked you to define a challenge you wanted
				to focus on solving. This statement essentially gets used as the "How Might We" statement, so
				I felt that was slightly misleading, but it did then give a list of 10 solutions that could be
				taken to address the challenge.
			</li>
		</ol>
		<p>
			This was all done using QoQo's documentation (<a
				href="https://www.figma.com/community/plugin/1189158575928509194/qoqo-ai-ai-generated-wireframe-ux-personas-journey-mapping-sitemap-and-copywriting"
				>documentation linked here</a
			>).
		</p>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Evaluation</h2>
		<p>
			To evaluate the effectiveness of each part of my testing, I'll be rating the overall end
			product each part of the test produced on a scale of 1 to 10, with 1 being completely
			ineffective and 10 being extremely effective. Each section will have it's own definition of
			effectiveness.
		</p>
		<ol>
			<li>
				<strong>Affinity Mapping:</strong> For affinity mapping, my effectiveness definition relies
				mostly on whether or not the groups made sense, as well as if the insights that came out of
				them were of quality. While the process of using it was very quick and simple, the map it
				produced put the sticky notes into three groups, of which were not very specific and did not
				seem particularly of interest. For instance, one group was titled "Pick Up Time", which
				wasn't really representative of the data under it. Another was titled "Buying from food
				truck supports local people", which would not have been useful for finding solutions for a
				food truck. It did not encapsulate the point of the sticky notes under it, either. Overall,
				the tool was not particularly effective.
				<strong>Effectiveness: 3/10</strong>
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
