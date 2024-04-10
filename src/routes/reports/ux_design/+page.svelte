<script lang="ts">
	import Challenges from '$lib/assets/Challenges.png';
	import Cluster from '$lib/assets/Cluster.png';
	import Interview from '$lib/assets/Screenshot 2024-04-10 001543.png';
</script>

<h1>UX Design and A.I.</h1>
<div class="section">
	<div class="section-card">
		<h2>Research Goal</h2>
		<p>
			In this report, I will be looking to find how A.I. tools help UX designers accomplish their
			job more easily. I am mostly looking to find how these tools can help facilitate the tedious
			parts of UX Design, such as organizing notes, creating interview scripts, and so on.
		</p>
	</div>
	<div class="section-card">
		<h2>Tool Researched</h2>
		<p>
			My research will focus on the tool, QoQo (pronounced "coco"), which is a plugin made to work
			with Figma. It was created with the intention to automate the process of creating user journey
			maps, generating affinity diagrams, writing interview scripts, an so on.
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
				Make an affinity map using notes taken from several user interviews and QoQo's "Affinity
				Mapping" tool. This tool allows you to either use a text transcript of a user interview or a
				group of sticky notes if you've already put your data into Figma. I chose to use the sticky
				notes I had from the project, which meant all I had to do was select all the sticky notes
				and hit "Cluster", which starts the grouping process. After a few seconds, it had finished
				grouping the items into three named groups.
			</li>
			<li>
				Make a interview script based off of some persona information and general interview topics
				with their "Use Interview" tool. This was more of a form where it asked you to input
				information like the age, gender, and occupation of a persona you are targeting, a general
				situation the user would be in that they would be interacting with your product, and some
				topics to ask questions about. After inputting all of that, it gave me a list of questions
				grouped by the different topics I had entered.
			</li>
			<li>
				Make a "How Might We" statement with potential solutions to solve the users issues with
				their "How Might We" tool. This tool only asked you to define a challenge you wanted to
				focus on solving. This statement essentially gets used as the "How Might We" statement, so I
				felt that was slightly misleading, but it did then give a list of 10 solutions that could be
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
			In this report, I will be looking to find how A.I. tools help UX Designers accomplish their
			job more easily. I am mostly looking to find how these tools can help facilitate the tedious
			parts of UX Design, such as organizing notes, creating empathy maps, and so on.
		</p>
	</div>
	<div class="section-card">
		<h2>Conclusion</h2>
		<p>
			In this report, I will be looking to find how A.I. tools help UX Designers accomplish their
			job more easily. I am mostly looking to find how these tools can help facilitate the tedious
			parts of UX Design, such as organizing notes, creating empathy maps, and so on.
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
		</div>
	</div>
</div>
