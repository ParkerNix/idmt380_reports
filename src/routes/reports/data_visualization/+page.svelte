<script>
	import Tableimg from '$lib/assets/Data Visualization/table.png';
	import CodingTest from '$lib/assets/Data Visualization/codingtest.png';
	import StylingTest from '$lib/assets/Data Visualization/stylingtest.png';
</script>

<h1>ChatGPT and Graphs</h1>
<div class="section">
	<div class="section-card">
		<h2>Research Goal</h2>
		<p>
			In this report, I seek to answer the question; "To what extent can ChatGPT predict the most
			suitable graph type for visualizing tabular data sets, and how accurately can it generate and
			style reusable React components to implement these visualizations?"
		</p>
		<p>
			To start, my hypothesis was that ChatGPT would be able to create functional code for the graph
			and style it accurately, but would be unable to make a good judgment on what graph to use.
		</p>
	</div>
	<div class="section-card">
		<h2>Tool Researched</h2>
		<p>
			I used ChatGPT which I have been using it in my daily coding activities, and Chart.js. A while
			back, I did a project that required me to use Chart.js to visualize different data sets. I
			personally found this to be a struggle in using the right charts and getting the right
			styling, so I wanted to see if ChatGPT could have done it faster, as my current job could also
			benefit from data visualization in our codebase.
		</p>
	</div>
	<div class="section-card">
		<h2>Implementation and Testing</h2>
		<p>To examine ChatGPT's ability to pick, code, and style graphs:</p>
		<ol>
			<li>Generate a table of data to feed to ChatGPT</li>
			<li>Ask ChatGPT for the best graph to use for this data</li>
			<ol>
				<li>
					If it returns a graph type that is appropriate for the data, continue; In the case the
					graph is not correct, tell it to use a more appropriate chart in the next step
				</li>
			</ol>
			<li>
				Ask it to generate a React component that renders the graph using Chart.js. It should be
				reusable and take any variables necessary to create a chart from similar tables of data.
			</li>
			<li>
				Ask it to restyle the graph. The graph should use only the colors blue (#6DA8FF), yellow
				(#FFCE50), red (#FF8159), and green (#5FCCA0), should have a background color of #FDFCF1
				when hovered over, and should have all axes and legends labeled.
			</li>
		</ol>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Evaluation</h2>
		<p>The following section will cover each test and the outputs ChatGPT gave me:</p>
		<h3>Best Graph Test</h3>
		<ul>
			<li>
				<strong>Prompt:</strong> “I want to analyze this data as a graph, what graph would suit the data
				the best if I wanted to see and compare how each person's time changed over the months?”
			</li>
			<li>
				<strong>Output:</strong>
				<p>
					For comparing how each person's time changed over the months, a line graph would be a
					suitable choice. In this graph, you can have the months on the x-axis and the time taken
					for the first elimination on the y-axis. Each person (Parker, Sarah, and Katie) would have
					their own line plotted on the graph, allowing you to easily compare their performance over
					time. Would you like me to create such a graph for you, or do you have specific
					preferences or requirements for the graph?
				</p>
			</li>
			<li>
				<strong>Outcome:</strong>
				<p>
					ChatGPT chose an appropriate graph to compare how each person's time changed over the
					months, and clearly explained why it is a good fit.
				</p>
			</li>
		</ul>
		<img src={Tableimg} alt="The table of data I started with" />
		<hr />
		<h3>Examples Test</h3>
		<ul>
			<li>
				<strong>Prompt:</strong> “I want to be able to use a graph like that in my React project, but
				I'd like a reusable component that can accept variables to make a new graph each time I call
				it. Would you be able to create such a component using Chart.js?”
			</li>
			<li>
				<a
					href="https://github.com/ParkerNix/graph-tests/blob/CodingTest/src/components/line.tsx"
					target="_blank">Link to Generated Code</a
				>
			</li>
			<li>
				<strong>Outcome:</strong>
				<p>
					ChatGPT was able to create a component that rendered a line chart that takes all the
					variables it would need. I did have to ask it to redo the component though, as it did not
					render at first. Here is the second round of prompting:
				</p>
				<p>
					“When attempting to use this code, I get the error: Error: Canvas is already in use. Chart
					with ID '0' must be destroyed before the canvas with ID '' can be reused.”
				</p>
				<p>
					“The error message indicates that you're trying to render a new Chart instance on a canvas
					element that is already being used by another Chart instance. To resolve this, you need to
					ensure that any existing Chart instance is destroyed before rendering a new one."
				</p>
				<p>After this, the graph worked as expected.</p>
			</li>
		</ul>
		<img src={CodingTest} alt="The graph after being generated" />
		<hr />
		<h3>Graph Styling Test</h3>
		<ul>
			<li>
				<strong>Prompt:</strong> “Okay, so I'd like to do some styling to the graph. The graph should
				use only the colors blue (#6DA8FF), yellow (#FFCE50), red (#FF8159), and green (#5FCCA0), should
				have a background color of #FDFCF1 when hovered over, and should have all axes and legends labeled.
				Could you regenerate the component with that in mind?”
			</li>
			<li>
				<strong>Output:</strong>
				<a
					href="https://github.com/ParkerNix/graph-tests/blob/CodingTest/src/components/line.tsx"
					target="_blank">Link to Generated Code</a
				>
			</li>
			<li>
				<strong>Outcome:</strong>
				<p>
					This solution did correctly style the graph, but it was not able to assign a background
					color on hover. Instead, it told me that I could achieve it with CSS. While it isn't
					wrong, I would have appreciated it giving me CSS code to achieve it.
				</p>
			</li>
		</ul>
		<img src={StylingTest} alt="The graph with styling applied" />
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Conclusion</h2>
		<p>
			The tests showed that ChatGPT was able to correctly find an appropriate chart for the data,
			but hit a snag trying to code out and style the graph. It was able to correct most issues or
			at least tell me how to fix it myself. Overall, I would say that my hypothesis was largely
			backwards, but it can predict the most suitable graph type for visualizing tabular data sets,
			and it can mostly generate and style reusable React components.
		</p>
	</div>
</div>
