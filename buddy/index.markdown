---
layout: default
title: "buddy"
date: 2014-06-11 22:10
comments: true
sharing: true
footer: true
category: buddy
---

<div id="front-wrapper">
 <div class="dummy">
	<center>
		
		<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
		<!-- responsive -->
		<ins class="adsbygoogle responsive"
			 style="display:inline-block"
			 data-ad-client="ca-pub-5594910991615008"
			 data-ad-slot="9295527574"></ins>
		<script>
			(adsbygoogle = window.adsbygoogle || []).push({});
		</script>
	</center>
 </div>
 
  <div class="container">
  <div style="width:50%;margin-left:auto;margin-right:auto;text-align:center">
	<h1 style="font-size:300%">buddy</h1>
	<br/>
  </div>
  <div style="overflow:auto">
	<div style="width:80%;margin-left:10%"><center><img src="http://anthonyrotio.com/rotiofood/buddy/buddy.gif"/></center></div>
	<div class="bud1" style="width:80%;margin-left:10%;text-align:center"><br/>A sourdough starter is fed flour and water twice a day and left open to recruit natural yeast, grow, and develop complex flavors. <br/> The best breads are usually made from starters that have been around for many years. <br/> Buddy is a sourdough starter... with a bit of a twist: <br/> Since he was born in January 2014, <u>Buddy has only ever been fed Bread Flour and Budweiser </u> <br/>(and a little hit of yeast to jump start him at the beginning). <br/>The flavor is delicious and getting better every day, check back here to see what Buddy's been up to!</div>
  </div>
{% assign cat = page.category %}
<br/><br/>
<div class="row" id="post-container">
  <div style="width:90%;margin-left:auto;margin-right:auto;text-align:center">
    <h3>{{ cat }}'s drank <span class="budweiser_count"></span> Budweisers and counting... <br/><br/>Buddy's spawn:</h3>
  </div>
  {% assign index = true %}
  <div>
      {% for post in site.categories.[cat] %}
	  <section>
		<h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
		{{ post.excerpt }}
	  </section>
      {% endfor %}
  </div>
</div>
</div>
</div>
<script>var oneDay = 24*60*60*1000; // hours*minutes*seconds*milliseconds
var firstDate = new Date(2014,01,01);
var secondDate = new Date();

var diffDays = Math.round(Math.abs((firstDate.getTime() - secondDate.getTime())/(oneDay)));
var beers = diffDays/2;
$('.budweiser_count').text(beers);
</script>
