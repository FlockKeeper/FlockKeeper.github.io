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
					<h1 id="countdownDays">&nbsp;</h1>
					<p>Days</p>
				</td>
				<td>
					<h1 id="countdownHours">&nbsp;</h1>
					<p>Hours</p>
				</td>
				<td>
					<h1 id="countdownMinutes">&nbsp;</h1>
					<p>Minutes</p>
				</td>
				<td><div>
					<h1 id="countdownSeconds">&nbsp;</h1>
					<p>Seconds</p>
				</div></td>
			</tr>
			<tr>
				<td>
				</td>
			</tr>
		</table>
	</div>

	<div id="tabsMain" class="mainInformation">
		<ul class="nav nav-tabs" style="margin:0;">
		  <li id="tabProgress" class="active">
			<a href="#null">Current Progress</a>
		  </li>
		  <li id="tabFeedback"><a href="#null">Offer Feedback</a></li>
		  <li id="tabSocialMedia"><a href="#null">Follow Us</a></li>
		  <li id="tabNewsletter"><a href="#null">Stay Informed</a></li>
		  <li id="tabAboutUs"><a href="#null">About Us</a></li>
		</ul>
		
		<div id="mainInformationPages" class="mainInformationPages">
		
			<div id="divtabProgress">
				<div>We're about <span id="percentDone">5</span>% finished!</div>

				<div class="progress" style="margin:20px;">
				  <div class="bar" style="width: 5%;"></div>
				</div>
				
				<table border="0" cellspacing="0" cellpadding="0" style="width:100%;">
					<tr>
						<td style="vertical-align:top; width:250px;">
							<a href="{{ BASE_PATH }}/images/TwitterIcon.png" target="_blank"><img border="0" src="{{ BASE_PATH }}/images/TwitterIcon.png" alt="Logo" style="width:250px; height:250px;"/></a>
						</td>
						<td style="padding-left:20px; vertical-align:top;">
							<h2>What we're working on now:</h2>
				
							<ul>
								<li>Gathering feedback from early adopters (That's you!)</li>
								<li>Planning for and designing core features</li>
								<li>Implementing specific features for select clients</li>
							</ul>
							
							<div class="divBlogPosts">
								<h2>Blog Posts Here ...</h2>
								<p>Blah blah blah blah blah blah blah blah blah.</p>
				
								<h2>Blog Posts Here ...</h2>
								<p>Blah blah blah blah blah blah blah blah blah.</p>
				
								<h2>Blog Posts Here ...</h2>
								<p>Blah blah blah blah blah blah blah blah blah.</p>
							</div>
						</td>
					</tr>
				</table>
			
			</div>
		
			<div id="divtabFeedback" style="display:none;">
				<h2>Our New Service</h2>

				<p>Flock Keeper is intended to be an all-in-one solution for church, charity, and non-profit organization management. We are reaching out to our community of potential users well before development begins to see what features would be most valueable to those users.</p>

				<p>While we will have to charge a premium for some services, our intent is to offer many features at little or no cost for smaller organizations. Your feedback will help us prioritize our development efforts and determine a fair pricing scheme.</p>
				
				<p>Please take a moment to complete the following 10-question survey.</p>
				
				<div id="surveyMonkeyInfo"><div><script src="http://www.surveymonkey.com/jsEmbed.aspx?sm=6FbEvTP1RzNXlWP_2bpI_2fy6g_3d_3d"> </script></div>Create your free online surveys with <a href="https://www.surveymonkey.com">SurveyMonkey</a> , the world's leading questionnaire tool.</div>
			</div>
		
			<div id="divtabSocialMedia" style="display:none;">
				<ul>
					<li>Twitter</li>
					<li>Facebook</li>
					<li>Google+</li>
					<li>RSS Feed</li>
				</ul>
			</div>
		
			<div id="divtabNewsletter" style="display:none;">
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
		
			<div id="divtabAboutUs" style="display:none;">
				<p>About us.
				</p>
			</div>
		
		</div>
		
	</div>

</div>	

<script type="text/javascript">
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
	
	function onClickTabsMain($obj) {
		$("#mainInformationPages > div").hide();
		$("#tabsMain ul li").removeClass("active");
		$obj.addClass("active");
		$("#div" + $obj.attr("id")).show();
	}

</script>

