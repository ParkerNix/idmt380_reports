<h1>Codiumate and Test Cases</h1>
<div class="section">
	<div class="section-card">
		<h2>Research Goal</h2>
		<p>
			In this report, I will be examining how effective Codiumate is at writing test code for short
			functioning or non-functioning code and more complex functioning or non-functioning code
			written in Typescript. I'll be basing my findings off of a 1 to 10 scale that rates the
			effectiveness of each test.
		</p>
		<p>
			To start, my hypothesis was that Codiumate would be great at testing simple, short code that
			was functioning. However, I thought it would not be able to write test cases if the code was
			broken and it might struggle to write them when the functions became more complex. Overall, I
			was expecting an average rating of 6/10.
		</p>
	</div>
	<div class="section-card">
		<h2>Tool Researched</h2>
		<p>
			Codiumate, an extension created by CodiumAI, is a tool for building tests for your code and
			insuring the security of it. Given a function, it can produce multiple test cases that aim to
			target different potential issues with your code. Writing tests can be helpful, but also very
			tedious and demotivating, so I wanted to use this tool to see how easy it is to test code
			snippets.
		</p>
	</div>
	<div class="section-card">
		<h2>Implementation and Testing</h2>
		<p>To examine the effectiveness of Codiumate:</p>
		<ol>
			<li>
				<strong>Create 4 samples of code:</strong>
				<ol>
					<li>A shorter, functioning function</li>
					<li>The first function, but with an error in it</li>
					<li>A longer, more complex function</li>
					<li>The third function, but with an error in it</li>
				</ol>
			</li>
			<li>
				Ask Codiumate to <strong>make test cases for each function.</strong>
			</li>
			<li>
				<strong>Evaluate the test case sets (2 cases each) on a 1 to 10 scale</strong> in terms of accuracy
				and effectiveness of the test cases.
			</li>
		</ol>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Evaluation</h2>
		<p>
			<a
				href="https://github.com/ParkerNix/pcn23_test-cases/blob/main/test-gen-IDMT380.ts"
				target="_blank">Link to functions used</a
			> | The following section will cover each function I created and the test cases Codiumate produced
			in return:
		</p>
		<ol>
			<li>
				<strong>Short Functioning</strong> |
				<a
					href="https://github.com/ParkerNix/pcn23_test-cases/blob/main/shortgood.ts"
					target="_blank">link to test cases</a
				>
				<ul>
					<li>
						<strong>Function:</strong>
						<ul>
							<li>
								<strong>Description:</strong> ”AddNumbers” takes two number inputs, "a" and "b"and calculates
								the sum of ”a” and ”b”, storing it in a variable "c". The value of "c" is then logged
								to the console.
							</li>
						</ul>
					</li>
					<li>
						<strong>Thoughts:</strong>
						<ul>
							<li>The first test is pretty accurate and tests the main purpose of the function</li>
							<li>
								The second test makes the expected value the max safe integer - 3, which would never
								equal (the max safe integer - 1) + (the max safe integer - 2)
							</li>
							<li>Seems like it can get a bit too specific for it's own good</li>
							<li><strong>Rating: 7/10</strong></li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<strong>Short Non-Functioning</strong> |
				<a
					href="https://github.com/ParkerNix/pcn23_test-cases/blob/main/shortbad.ts"
					target="_blank">link to test cases</a
				>
				<ul>
					<li>
						<strong>Function:</strong>
						<ul>
							<li>
								<strong>Description:</strong> ”BadAddNumbers” takes two number inputs, "a" and "b"and
								calculates the sum of ”a” and ”b”, storing it in a variable "c". However the value of
								an undefined variable "d" is then logged to the console, which is incorrect.
							</li>
						</ul>
					</li>
					<li>
						<strong>Thoughts:</strong>
						<ul>
							<li>
								The first test is once again accurate and tests the main purpose of the function
							</li>
							<li>
								The second test now uses 0 and a positive number, which is cool but maybe slightly
								redundant
							</li>
							<li><strong>Rating: 9/10</strong></li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<strong>Complex Functioning</strong> |
				<a
					href="https://github.com/ParkerNix/pcn23_test-cases/blob/main/complexgood.ts"
					target="_blank">link to test cases</a
				>
				<ul>
					<li>
						<strong>Function:</strong>
						<ul>
							<li>
								<strong>Description:</strong> "DeleteMatch" takes two arrays and checks that they are
								arrays of strings and of the same length. Should either be false, it will throw an error.
								Then, it loops through each item in the first array and tries to find a matching string.
								The first matching string it finds, it takes the index of it and stores it. Finally,
								it takes the two arrays and, using the index found from before, deletes the matching
								string form both. If no such string is found in any item in the arrays, it will throw
								an error.
							</li>
						</ul>
					</li>
					<li>
						<strong>Thoughts:</strong>
						<ul>
							<li>
								The first test is once again accurate and tests the main purpose of the function
							</li>
							<li>
								The second test tries to use the function with an empty array, which is not
								something I would immediately think to test but is a good security measure
							</li>
							<li><strong>Rating: 10/10</strong></li>
						</ul>
					</li>
				</ul>
			</li>
			<hr />
			<li>
				<strong>Complex Non-Functioning</strong> |
				<a
					href="https://github.com/ParkerNix/pcn23_test-cases/blob/main/complexbad.ts"
					target="_blank">link to test cases</a
				>
				<ul>
					<li>
						<strong>Function:</strong>
						<ul>
							<li>
								<strong>Description:</strong> "BadDeleteMatch" takes two arrays and checks that they
								are arrays of strings and of the same length. Should either be false, it will throw an
								error. Then, it loops through each item in the first array and tries to find a matching
								string. The first matching string it finds, it takes the string that matched and stores
								it. Finally, it takes the two arrays and, using the index found from before, attempts
								to delete the matching string form both. However, the index is of type "string", making
								that impossible.
							</li>
						</ul>
					</li>
					<li>
						<strong>Thoughts:</strong>
						<ul>
							<li>Both tests are once again accurate and effective in testing possible flaws</li>
							<li>
								I'm finding the second test to have a tendency to be a bit of a wild card; it can
								test a lot of things you may not immediately think of, which I think is really nice
								as you can use it to learn a bit as well
							</li>
							<li><strong>Rating: 10/10</strong></li>
						</ul>
					</li>
				</ul>
			</li>
		</ol>
		<hr />
		<p>Final average: 9.5/10</p>
	</div>
</div>

<div class="section">
	<div class="section-card">
		<h2>Conclusion</h2>
		<p>
			Codiumate can be very accurate and creative in making test cases. I was quite shocked at how
			capable it was at understanding what the code was for and making a variety of cases based off
			that. In addition, even code with errors, which I thought for sure would be it's downfall,
			were tested in a way that was appropriate, though the function would have failed the test.
			Overall, I find that Codiumate is a highly effective tool for writing test cases of any kind.
			In the future, I will certainly be using this tool to help at work and trying to find a way to
			make integration tests that much less of a hassle.
		</p>
	</div>
</div>
