---
permalink: /index.html
layout: main
title: Institute for Research and Innovation in Software
bgimage: assets/images/Tprime-200pu-PhaseII-black-arctic-main-image.jpg
barelogo: assets/images/IRIS-HEP-Logo.png
---
<h3>Computational and data science research to enable discoveries in fundamental physics</h3>
<br>
IRIS-HEP is a software institute funded by the National Science Foundation. It aims to develop the state-of-the-art software cyberinfrastructure required for the challenges of data intensive scientific research at the High Luminosity Large Hadron Collider (HL-LHC) at CERN, and other planned HEP experiments of the 2020's. These facilities are discovery machines which aim to understand the fundamental building blocks of nature and their interactions. [Full Overview](/about/overview.html)
<br><br>
The IRIS-HEP project was funded on 1 September, 2018, and is ramping up its activities. 

<br>
<h4>Upcoming Events:</h4>
IRIS-HEP team members are involved in organizing the following events:


<br>

<div class="container">
  <div id="accordion">
    
	{% assign event_items = site.data.events %}
	{% assign event_number = 0 %}
	{% for event_hash in event_items  %}
		{% assign event = event_hash[1] %}
		{% if event.status == 'current' %}
			{% assign event_number = event_number | plus: 1 %}
			{% assign event_id = event_number | downcase %}
	
		
			<div class="card">		
				<div class="card-header">
					<a class="card-link" data-toggle="collapse" href="#{{ "collapse" | append: event_id }}">
						{{ event.dates }} - {{ event.name }}
					</a>
				</div>
				<div id="{{ "collapse" | append: event_id }}" class="collapse" data-parent="#accordion">
					<div  class="card-body">
						<ul>
							<li> <b>Venue: </b><i>{{ event.location }}</i> </li>
							<li> <a href="{{ event.website }}">Website</a> </li>
						</ul>
					</div>
				</div>
			</div>
				
		{% endif %}
	{% endfor %}
	  
  </div>
	
</div>

<br>

<h4>Past Events:</h4>
<br>


<div class="container">
  <div id="accordion2">
    
	{% assign event_items = site.data.events %}
	{% assign event_number = 0 %}
	{% for event_hash in event_items  %}
		{% assign event = event_hash[1] %}
		{% if event.status == 'past' %}
			{% assign event_number = event_number | plus: 1 %}
			{% assign event_id = event_number | downcase %}
	
		
			<div class="card">		
				<div class="card-header">
					<a class="card-link" data-toggle="collapse" href="#{{ "Pcollapse" | append: event_id }}">
						{{ event.dates }} - {{ event.name }}
					</a>
				</div>
				<div id="{{ "Pcollapse" | append: event_id }}" class="collapse" data-parent="#accordion2">
					<div  class="card-body">
						<ul>
							<li> <b> Venue: </b> <i>{{ event.location }}</i> </li>
							<li> <a href="{{ event.website }}">Website</a> </li>
						</ul>
					</div>
				</div>
			</div>
				
		{% endif %}
	{% endfor %}
	  
  </div>
	
</div>


<


