---
permalink: /news
layout: default
title: accordion template

---



<div class="container">
  <h4>Accordion Template</h4>
  
  <p>First accordion is openned by default, the two others are collapsed - this is an example only. This accordion does not require custon JS/jQuery scrips, it relies on the standard ones 
   as well as bootstrap, so if one of those is modified this might affect the accordion appearance/performance.</p>
  <p><strong>Note:</strong> The <strong>data-parent</strong> attribute makes sure that all collapsible elements under the specified parent will be closed when one of the collapsible item is shown.</p>
  <div id="accordion">
  
    <div class="card">
	  <div class="card-header">
        <a class="card-link" data-toggle="collapse" href="#collapseOne">
          Collapsible Group Item #1
        </a>
      </div>
      <div id="collapseOne" class="collapse show" data-parent="#accordion">
        <div class="card-body">
          Text of block 1.
        </div>
      </div>
    </div>
	
	<div class="card">
      <div class="card-header">
        <a class="collapsed card-link" data-toggle="collapse" href="#collapseTwo">
        Collapsible Group Item #2
      </a>
      </div>
      <div id="collapseTwo" class="collapse" data-parent="#accordion">
        <div class="card-body">
          Text of block2.
        </div>
      </div>
    </div>
	
    <div class="card">
      <div class="card-header">
        <a class="collapsed card-link" data-toggle="collapse" href="#collapseThree">
          Collapsible Group Item #3
        </a>
      </div>
      <div id="collapseThree" class="collapse" data-parent="#accordion">
        <div class="card-body">
          Text of block 3.
        </div>
      </div>
    </div>
	
  </div>
</div>
    
