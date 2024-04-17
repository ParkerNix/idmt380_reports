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
</div>

<div class="section">
	<div class="section-card">
		<h2>Implementation and Testing</h2>
		<p>To examine this tool, I followed these steps per test:</p>
		<ol>
			<li>
				<strong>Give Framer AI a prompt</strong> with details on tone and what should be included.
			</li>
			<hr />
			<li>
				<strong>Hit “Generate”</strong> and let the AI work
			</li>
			<hr />
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

<div class="section">
	<div class="section-card">
		<h2>Raw Prompts/Outputs</h2>
		<h3>Affinity Map Output</h3>
		<p>
			Pick up time 1. Pick up ASAP with estimated wait time 2. Choose pick up time 3. Offer to
			remember payment method so user doesn't have to put in the same payment information again 4.
			Shows steps: Order Placed, Working on Order, Order is ready for pickup 5. Being able to save
			favorite items 6. Show if items are in stock 7. Option to add additional notes or special
			instructions 8. Display all menu customization options such as adding onions, salt, pepper,
			ketchup, etc while checking out 9. Online Payments - Different payment options allowed such as
			Paypal, Credit and Debit Cards 10. Customer Service - Adding messages like thank you for
			ordering, show customer appreciation Small business 1. More personal experience 2. User like
			to support small businesses 3. Owner Interaction - Users will still be interacting with owners
			and receiving their customer service through pick up 4. Many users are students who are more
			likely to be using their phones and apps 5. Taste over messy presentation 6. Will stop going
			if food quality goes down 7. Won't go if customer service is bad 8. Some won't go if the
			presentation of the food does not look good 9. Some customers don't care about the service if
			the food is good 10. Will avoid if lines are too long - preordering on the app would help
			shorten lines 11. Commuters need cheap food if they are on campus all day. 12. Users that live
			on campus are more likely to order on the weekends 13. Low prices - organizing from low to
			high 14. Close location to classes 15. Going to the same trucks for specific menu items 16.
			Users are workers 17. Many users go to trucks based on friends' recommendations - Share button
			18. Online Reviews - Can include reviews from both the internet and ability to add reviews in
			the app 19. Eat between classes - An app would allow users to order right after their classes
			on their walk to the truck 20. Hot and fresh food 21. Good tasting food - Including photos to
			highlight the food 22. Users usually lunch time can be the busy around this time 23. Customers
			form a relationship with the staff 24. We have an established brand 25. We are well known on
			campus 26. Both cash and digital payment options 27. Signature dish that they make better than
			others in the area Buying from food truck supports local people 1. Opens Early - 6 AM 2. Will
			avoid if it seems unhygienic 3. Might be apprehensive to try a new place 4. If the staff isn't
			friendly or helpful the customer may not come back 5. Opens Early - 6 AM 6. Show most popular
			items
		</p>
		<hr />
		<h3>User Interview Script Prompt</h3>
		<ul>
			<li>
				<strong>Persona:</strong> 20 year old female; Lives in Philadelphia, PA; Is a student at a local
				university
			</li>
			<li>
				<strong>Scenario:</strong> The user wants to be able to get food on the go when they are between
				classes without a long wait time and for a low price.
			</li>
			<li>
				<strong>Topics:</strong> Price, Wait times, Favorite items, Desired features for an ordering
				app
			</li>
		</ul>
		<h3>User Interview Script Output</h3>
		<p>
			Thanks for accepting and taking the time to meet with us today. I'm (name and position). I'm
			from [company name]. We are conducting this interview to understand our customers better. A
			couple of points before we get started. For one, in today's conversation, we will be asking
			questions about your experience and the goal is to learn about your thoughts and your ideas.
			There are no right or wrong answers, just answer as openly and honestly as you can. The
			interview will take about [Enter duration]mins. All information will be kept confidential and
			not attributed at the individual level. Lastly, before we get started, we do like to record
			these sessions. These recordings are for internal use only and will not be shared outside of
			the project team. So if it's ok with you I'll press record and we can get started. Price
			questions: 1. How important is the price of food when you are looking for something to eat
			between classes? 2. Do you have a specific budget in mind when it comes to buying food on the
			go? 3. What factors do you consider when determining if a food item is reasonably priced? 4.
			Are you willing to pay a premium for healthier food options? 5. How does the price of food
			affect your decision to try new places? Wait times questions: 1. How much time are you willing
			to wait for your food between classes? 2. What do you usually do to pass the time while
			waiting for your food? 3. Have you ever left a food establishment because the wait time was
			too long? 4. What do you think is a reasonable wait time for fast food? 5. Are there any
			specific strategies you use to avoid long wait times? Favorite items questions: 1. What are
			your go-to food items when you are in a hurry? 2. Do you have any dietary restrictions or
			preferences that influence your choice of food items? 3. Are there any specific food items
			that you always crave? 4. How often do you try new food items? 5. Do you have any favorite
			food establishments near your university? Desired features for an ordering map questions: 1.
			What features would you like to see in an ordering map for food establishments near your
			university? 2. How important is it for you to see real-time wait times on the ordering map? 3.
			Would you find it helpful to have filters for price range and food type on the ordering map?
			4. Are there any specific features that you think would make the ordering map more
			user-friendly? 5. Do you have any suggestions for improving the overall experience of using an
			ordering map? Thank you for taking the time to speak with us today. Your insights and
			experiences are invaluable in helping us design solutions that truly meet the needs. We
			appreciate your candid responses and willingness to share your thoughts with us. Thank you
			again for your participation in this interview.
		</p>
		<hr />
		<h3>How Might We Prompt</h3>
		<p>
			The user wants to be able to get food on the go when they are between classes without a long
			wait time and for a low price.
		</p>
		<h3>How Might We Solutions</h3>
		<ul>
			<li>
				1. Implement a mobile ordering system that allows users to pre-order their food and pick it
				up at a designated time.
			</li>
			<li>
				2. Create a dedicated express lane for quick service and shorter wait times for users who
				are in a hurry.
			</li>
			<li>
				3. Offer a selection of pre-packaged grab-and-go meals that are ready to be picked up
				without any wait time.
			</li>
			<li>
				4. Introduce self-service kiosks where users can place their orders and pay without having
				to wait in line.
			</li>
			<li>
				5. Provide a menu with limited options specifically designed for quick service and efficient
				preparation.
			</li>
			<li>
				6. Partner with local food delivery services to offer on-campus delivery options for users
				who can't leave their classes.
			</li>
			<li>
				7. Implement a loyalty program that rewards users for frequent visits and offers discounts
				on their orders.
			</li>
			<li>
				8. Offer a student discount for users who present their student ID, making the food more
				affordable for them.
			</li>
			<li>
				9. Create a designated seating area for users who want to eat their food on the go, with
				convenient tables and chairs.
			</li>
			<li>
				10. Provide clear signage and directions to help users navigate the food options and find
				what they need quickly.
			</li>
		</ul>
	</div>
</div>
