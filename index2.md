---
layout: page
---
{% include JB/setup %}

<div class="mainContent">
	<h2>We're Building Something Great ...</h2>
	
	<p>If all goes as planned, we'll be launching this service in:</p>
	
	<div class="mainCountdown">
		<table border="0" cellspacing="0" cellpadding="0" style="width:100%;">
			<tr>
				<td>
					<h1 id="countdownDays">59</h1>
					<p>Days</p>
				</td>
				<td>
					<h1 id="countdownHours">23</h1>
					<p>Hours</p>
				</td>
				<td>
					<h1 id="countdownMinutes">59</h1>
					<p>Minutes</p>
				</td>
				<td><div>
					<h1 id="countdownSeconds">59</h1>
					<p>Seconds</p>
				</div></td>
			</tr>
			<tr>
				<td>
				</td>
			</tr>
		</table>
	</div>

	<div class="mainInformation">
		<ul class="nav nav-tabs" style="margin:0;">
		  <li class="active">
			<a href="#">Current Progress</a>
		  </li>
		  <li><a href="#">Offer Feedback</a></li>
		  <li><a href="#">Follow Us</a></li>
		  <li><a href="#">Stay Informed</a></li>
		</ul>
		
		<div class="mainInformationPages">
		
			<div id="divProgress">
				<div>We're about <span id="percentDone">5</span>% finished!</div>

				<div class="progress" style="margin:20px;">
				  <div class="bar" style="width: 5%;"></div>
				</div>

				<h2>What we're working on now:</h2>
				
				<ul>
					<li>Gathering feedback from early adopters (That's you!)</li>
					<li>Planning for and designing core features</li>
					<li>Implementing specific features for select clients</li>
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

</div>	

<script>
	var end = new Date('11/15/2014 10:00 AM');

	var _second = 1000;
	var _minute = _second * 60;
	var _hour = _minute * 60;
	var _day = _hour * 24;

	function showRemaining() {
		var now = new Date();
		var distance = end - now;
		if (distance < 0) {
			distance = 0;
			clearInterval(timer);
		}
		
		$("#countdownDays").text(Math.floor(distance / _day));
		$("#countdownHours").text(Math.floor((distance % _day) / _hour));
		$("#countdownMinutes").text(Math.floor((distance % _hour) / _minute));
		$("#countdownSeconds").text(Math.floor((distance % _minute) / _second));
	}
	
	var timer;
	$(document).ready(function(){
		timer = setInterval(showRemaining, 1000);
	});

</script>

