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
<!--
		  <li id="tabNewsletter"><a href="#null">Stay Informed</a></li>
-->
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
								{% assign posts_collate = site.posts %}

								{% for post in posts_collate offset:0 limit:5 %}
									<hr/>
									
									<h2 style="margin-bottom:5px;"><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
									<div style="font-size:0.8em; margin-bottom:15px;">&nbsp;&nbsp;{{ post.date | date_to_long_string }}</div>
									
									<div>{{ post.content }}</div>
	
								{% endfor %}
							</div>
						</td>
					</tr>
				</table>
			
			</div>
		
			<div id="divtabFeedback" style="display:none;">
				<h2>What is Flock Keeper?</h2>

				<p>Flock Keeper is intended to be an all-in-one solution for church, charity, and non-profit organization management. We are reaching out to our community of potential users well before development begins to see what features would be most valuable to those users.</p>

				<h2>Why Another Service?</h2>
				
				<p>As software developers, we're constantly approached by folks with great ideas for new applications. One of the most common requests is for software that makes managing groups and events easier. Those requests typically come from churches and non-profit organizations who are looking for solutions that address their needs in a user-friendly way.</p>
				
				<h2>How Much Will It Cost?</h2>
				
				<p>While we will have to charge a premium for some services, our intent is to offer many features at little or no cost for smaller organizations. Your feedback will help us prioritize our development efforts and determine a fair pricing scheme.</p>
				
				<h2>Help Us!</h2>
				
				<p>Please take a moment to complete the following 10-question survey. Your feedback will help us make the service even better!</p>
				
				<p><a class="btn btn-primary" href="https://www.surveymonkey.com/s/866WMLJ" target="_blank">Take Our Survey</a></p>
			</div>
		
			<div id="divtabSocialMedia" style="display:none;">
				<div>
					<table border="0" cellspacing="0" cellpadding="0">
						<tr>
							<td style="vertical-align:top; white-space:nowrap; width:150px;">
								<a href="https://twitter.com/FlockKeeper" target="_blank"><img src="{{ BASE_PATH }}/images/social/Twitter.png" alt="Twitter"/> Twitter</a><br/>
								<a href="https://www.facebook.com/FlockKeeper" target="_blank"><img src="{{ BASE_PATH }}/images/social/Facebook.png" alt="Facebook"/> Facebook</a><br/>
								<a href="https://plus.google.com/u/0/b/115289891490487608586/115289891490487608586/posts" target="_blank"><img src="{{ BASE_PATH }}/images/social/GooglePlus.png" alt="Google Plus"/> Google+</a><br/>
								<a href="http://feeds.feedburner.com/FlockKeeper" target="_blank"><img src="{{ BASE_PATH }}/images/social/RSS.png" alt="RSS Feed"/> RSS Feed</a><br/>
								<a href="http://feedburner.google.com/fb/a/mailverify?uri=FlockKeeper&amp;loc=en_US" target="_blank"><img src="{{ BASE_PATH }}/images/social/Mail.png" alt="Email"/> Email</a>
							</td>
							<td style="vertical-align:top; text-align:left;">
								<h2>Social Media</h2>
								<p>If you want to know everything that's going on during the process of building Flock Keeper, this is the place to be. Scott and Joe will be using this space as a blog during the process.</p>
<!-- 
								<p>If you just want to know when we hit major milestones or when have an important announcement, click on the "Stay Informed" tab.</p>
-->
							</td>
						</tr>
					</table>
				</div>
			</div>
		
			<div id="divtabNewsletter" style="display:none;">
<!--
				<table border="0" cellspacing="0" cellpadding="0">
					<tr>
						<td style="vertical-align:top; white-space:nowrap; width:150px;">
							<a href="" target="_blank"><img src="{{ BASE_PATH }}/images/social/Mail.png" alt="Newsletter"/> Newsletter</a>
						</td>
						<td style="vertical-align:top; text-align:left;">
							<h2>Newsletter</h2>
							<p>If you would like to know about updates as they're made, sign up for our newsletter. You will receive progress reports via email as we meet major milestones or encounter significant delays.</p>
							<p>The newsletter will be less chatty than the "Follow Us" options.</p>
						</td>
					</tr>
				</table>
-->
			</div>
		
			<div id="divtabAboutUs" style="display:none;">
				<h3>Scott Carthel Escue <span style="font-size:0.75em;">@carth3l</span></h3>

				<p>Scott Escue has worked as a software developer for over 14 years. He thrives on learning new
				tools and technologies, and he loves finding new approaches to solving problems.</p>

				<p>Scott has been developing in Java for over 12 years on projects large
				and small. It's his bread and butter, having worked with most of the
				technologies in the Java EE stack and surrounding
				ecosystem of libraries and frameworks.</p>

				<p>Scott is well versed with building web 
				applications and the technologies that support the same - HTML, CSS,
				and JavaScript (which, of course, implies a healthy disdain for IE). 
				He enjoys using "new fangled" libraries and tools to build responsive, 
				cross-browser UIs.</p>

				<p>Scott has been dabbling in Ruby and Rails development for over 5 years.
				He uses Rails exclusively for all the web applications he builds outside 
				his full time gig. He hasn't had the opportunity to work with Rails full time, 
				so he makes no claims of mastery. But, he loves the sense of productivity that 
				Rails affords when solving complex problems.</p>

				<p>Scott started his career building Oracle client-server applications, and
				has worked with Oracle databases in varying capacities ever since. He has also
				worked with a number of other databases, including MySQL, PostgreSQL, and
				several other lighter options such as Apache Derby and H2. Scott strives to
				build ANSI compliant SQL and vendor-neutral data integration to the greatest extent
				possible.</p>

				<p>He Lives with his family in Alabama.</p>

				<h3>Joseph Barrett Hall <span style="font-size:0.75em;">@groundh0g</span></h3>

				<p>Joe Hall has been a professional software developer for nearly 25 years.</p>

				<p>He worked as a programmer for Microsoft and IBM and he was the software architect 
				for a Fortune 500 bank. He was the CTO of a ticket sales and servicing company 
				and he started his own consulting company in 2006.</p>

				<p>Joe makes his living writing desktop, web, and mobile device applications for 
				businesses and governmental agencies, but game programming is his passion, and 
				it was gaming that got him into programming in the first place.</p>

				<p>He was a member of the original Xbox team and he joined the Visual Studio .NET team 
				just after the Xbox was released in 2001. Joe is the author of XNA Game Studio 
				Express: Developing Games for Windows and the Xbox 360, which was published in 2007.</p>

				<p>Joe also dabbles in sketching, cartooning, and creating 3D models. When you see his 
				artistic creations, you'll understand why he makes his living as a programmer.</p>

				<p>He Lives with his family in Alabama.</p>

				<h3>Team Sq&mu;all</h3>

				<p>With a combined experience of nearly four decades, Scott and Joe have been churning out 
				great apps for businesses and governmental agencies. Now, they're looking for a place to
				focus their copious free time.</p>
				
				<p><img src="{{ BASE_PATH }}/images/SquallLogo.png" alt="squall logo" /></p>
			</div>
		
		</div>
		
	</div>

</div>	

<script type="text/javascript">
	var end = new Date('06/15/2016 10:00 AM');

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

