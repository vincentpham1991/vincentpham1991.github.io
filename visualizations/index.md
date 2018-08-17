---
layout: page
title: Visualizations
excerpt: "Data Scientist"
modified: 2014-08-08T19:44:38.564948-04:00
---

<style type="text/css" media="screen">
.photo-grid {
	list-style: none;
	margin: 1em auto;
	max-width: 1106px;
	padding: 0;
	text-align: center;
}


.photo-grid li {
	display: inline-block;
	height: 163px;
	line-height: normal;
	margin: 1em;
	transition: all 500ms;
	width: 289px;
}


.photo-grid img {
	display: block;
	height: auto;
	transition: all 300ms;
	max-width: 100%;
}

.photo-grid li:hover img {
	-webkit-transform: scale(1.4);
}

.photo-grid figure {
	height: 163px;
	margin: 0;
	overflow: hidden;
	position: relative;
	width: 289px;
}

.photo-grid figcaption {
	background: rgba(0,0,0,0.8);
	color: white;
	display: table;
	height: 100%;
	left: 0;
	opacity: 0;
	position: absolute;
	right: 0;
	top: 0;
	transition: all 300ms;
	transition-delay: 100ms;
	width: 100%;
	z-index: 100;
}

.photo-grid li:hover figcaption {
	opacity: 1;
}

.photo-grid figcaption p {
	display: table-cell;
	font-size: 1.5em;
	position: relative;
	top: -40px;
	width: 289px;
	text-align: center;
	transition: all 300ms ease-out;
	vertical-align: middle;
}

.photo-grid figcaption p:empty {
display: none;
}

.photo-grid li:hover figcaption p {
	-webkit-transform: translateY(40px);
}

.photo-grid br {
	display: none;
}
</style>


<ul class="photo-grid">
	<li>
		<a href="{{ site.url }}/blog/CrunchBase">
			<figure>
				<img src="{{ site.url }}/images/startup.png" alt="image">
				<figcaption><p>Startups</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="{{ site.url }}/blog/CPS">
			<figure>
				<img src="{{ site.url }}/images/public_school.png" alt="image">
				<figcaption><p>Chicago Public High School</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="{{ site.url }}/blog/WorldTravels">
			<figure>
				<img src="{{ site.url }}/images/world.png" alt="image">
				<figcaption><p>Travels</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="{{ site.url }}/blog/USATravels">
			<figure>
				<img src="{{ site.url }}/images/usa.png" alt="image">
				<figcaption><p>Travels in the USA</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="{{ site.url }}/blog/GreeceTravels">
			<figure>
				<img src="{{ site.url }}/images/greece.png" alt="image">
				<figcaption><p>Travels in Greece</p></figcaption>
			</figure>
		</a>
	</li>


<!-- 	<li>
		<a href="https://github.com/CaptainDataCrunch/ObjectDetection">
			<figure>
				<img src="{{ site.url }}/images/car_adaboost.png" alt="image"></a>
				<figcaption><p>Car Detection Using Adaboost</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="https://github.com/vincentpham1991/titanic/blob/master/Vincent_Spark_tutorial.ipynb">
			<figure>
				<img src="{{ site.url }}/images/titanic.png" alt="image"></a>
				<figcaption><p>Spark Tutorial with Titanic Data</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="{{ site.url }}/blog/LoanProsper">
			<figure>
				<img src="{{ site.url }}/images/prosper.png" alt="image"></a>
				<figcaption><p>Exploratory Analysis of Loan Data</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="https://github.com/vincentpham1991/SentimentAnalysis">
			<figure>
				<img src="{{ site.url }}/images/movie.jpg" alt="image"></a>
				<figcaption><p>Sentiment Analysis of Movie Reviews</p></figcaption>
			</figure>
		</a>
	</li>
	<li>
		<a href="https://github.com/vincentpham1991/PythonProjects/tree/master/StocksHeatMap">
			<figure>
				<img src="{{ site.url }}/images/stocks2.jpg" height="180" width="320" alt="image"></a>
				<figcaption><p> Heat Map of Stock Correlations</p></figcaption>
			</figure>
		</a>
	</li>	 -->
</ul>
