---
layout: page
title: Test
---
{% include JB/setup %}

<div class="mainHeader">
	<h1>This is the header</h1>
</div>

<div class="mainContent">
	<h1>We're building something great ...</h1>
	<p>If all goes as planned, we'll be launching this service in:</p>
	
	<div class="mainCountdown">
		<table border="0" cellspacing="0" cellpadding="0" style="width:100%">
			<tr>
				<td>
					<span id="countdownDays">59</span><br/>
					<p>Days</p>
				</td>
				<td>
					<span id="countdownHours">23</span><br/>
					<p>Hours</p>
				</td>
				<td>
					<span id="countdownMinutes">59</span><br/>
					<p>Minutes</p>
				</td>
				<td>
					<span id="countdownSeconds">59</span><br/>
					<p>Seconds</p>
				</td>
			</tr>
		</table>
	</div>

	<div class="mainInformation">
		<ul class="nav nav-tabs">
		  <li class="active">
			<a href="#">Current Progress</a>
		  </li>
		  <li><a href="#">Offer Feedback</a></li>
		  <li><a href="#">Follow Us</a></li>
		  <li><a href="#">Stay Informed</a></li>
		</ul>
		
		<div id="divProgress">
			<div>We're about <span id="percentDone">10</span>% finished!</div>

			<div class="progress">
			  <div class="bar" style="width: 10%;"></div>
			</div>

			<div>What we're working on now:</div>
			<ul>
				<li>Gathering feedback from early adopters (That's you!)</li>
				<li>Planning for and designing core features.</li>
				<li>Implementing specific features for select clients.</li>
			</ul>
			
			<div class="divBlogPosts">
				<h2>Blog Posts Here ...</h2>
				<p>Blah blah blah blah blah blah blah blah blah.<p>
				
				<h2>Blog Posts Here ...</h2>
				<p>Blah blah blah blah blah blah blah blah blah.<p>
				
				<h2>Blog Posts Here ...</h2>
				<p>Blah blah blah blah blah blah blah blah blah.<p>
			</div>
		</div>
		
		<div id="divFeedback" style="display:none;">
			<p>[Inspirational text and survey go here...]</p>
		</div>
		
		<div id="divSocialMedia" style="display:none;">
			<ul>
				<li>Twitter</li>
				<li>Facebook</li>
				<li>Google+</li>
				<li>RSS Feed</li>
			</ul>
		</div>
		
		<div id="divNewsletter" style="display:none;">
			<p>If you would like to know about updates as they're made, sign
			   up for our newsletter. You will receive progress reports via
			   email as we meet major milestones or encounter significant 
			   delays.
			</p>
			
			<ul>
				<li>Newsletter</li>
				<li>Facebook</li>
				<li>Google+</li>
				<li>RSS Feed</li>
			</ul>
		</div>
		
	</div>

</div>	
