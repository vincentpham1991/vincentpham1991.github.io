---
layout: page
title: Conference Talks
excerpt: "Data Scientist"
modified: 2017-05-21T19:44:38.564948-04:00
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
	top: -9px;
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
		<a href="https://www.usenix.org/conference/opml20/presentation/pham">
			<figure>
				<img src="{{ site.url }}/images/opml_ppml.png" alt="image">
				<figcaption><p>USENIX (OpML '20) - Privacy Preserving Machine Learning</p></figcaption>
			</figure>
		</a>
	</li>
    <li>
        <a href="https://www.youtube.com/watch?v=H7KfmNNkXiY&feature=emb_logo">
            <figure>
                <img src="{{ site.url }}/images/defcon_spectrum.png" alt="image">
                <figcaption><p>DEFCON (AI Village '20) - ML-Based Threat Monitoring and Detection</p></figcaption>
            </figure>
        </a>
	</li>

</ul>