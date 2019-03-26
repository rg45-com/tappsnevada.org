---
sheetrock_js: >
  <!-- Load Handlebars.js from CloudFlare's CDN. -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/handlebars.js/4.0.5/handlebars.min.js"></script>
  
  <script src="/assets/js/plugins/sheetrock/sheetrock.min.js"></script>
  
  <script lang="javascript">
  var mySpreadsheet = 'https://docs.google.com/spreadsheets/d/12UvjAbdh1OST2unXHNJfRauHnyhwy-FzZVk1cJSnUY0/edit#gid=0';
  
  var wallTemplate = Handlebars.compile($('#wall-template').html());
  
  $('#wall_list').sheetrock({
    url: mySpreadsheet,
    sql: "select A, C order by C desc",
    //fetchSize: 20,
    labels: ['NAMES', 'ID'],
    rowHandler: wallTemplate
  });
  </script>
  <style>
    #wall_list {
      display: grid;
      grid-template-columns: repeat(auto-fit, 225px);
      grid-gap: 10px;
      justify-items: stretch;
    }
    #wall_list p {
      padding: 5px;
    }
   /* #wall_list p:nth-child(3){
        margin-right: 0;
    } */

  </style>
layout: default
title: "Memorial Wall for Veterans Honored with Taps"
---

<div class="content-container wall">
  <div class="inner-page-banr">
  	<div class="container">
      	<h2><span>T.A.P.P.S. Memorial </span>Wall</h2>
      </div>
  </div>
  <div class="inner-sections">
  	<div class="container">
  		<div class="top-icon-box">
          	<img src="/assets/images/header-top.png" class="header-icon center-block">
          	<div class="top-bx-inner">
              	<h3>T.A.P.P.S. Memorial Wall</h3>
                <p>All Veterans honored by T.A.P.P.S. are memorialized here on our Wall.</p>
              </div>
          </div>
          <div class="clearall"></div>
          <p class="wall-p1">Search for your Veteran by holding CTRL then pressing F.</p>
          <div class="wall-blue-box">
          	<div class="inr-wall">
              	<div class="inr-wall-double">
              		<img src="/assets/images/wall-heading.jpg" class="wall-heading" alt="wall-heading">
                      <div class="clearall"></div>
                       <script id="wall-template" type="text/x-handlebars-template">
                        {% raw %}
                          <p>{{cells.NAMES}}</p>
                        {% endraw %}
                      </script>
                      <div id="wall_list" class="inner-cont">
                      <p>LEONARD WILLIAM CARPI</p>
                      </div>
                      <div class="clearfix"></div>
              	</div>
              </div>
          </div>
      </div>
  </div>
  <div class="donate-sec-3">
  	<div class="container">
      	<h4 class="strip-heading">T.A.P.P.S. NEVADA would appreciate <br><span>a simple financial contribution.</span></h4>
          <p>Please donate any amount you can here <br>(One time or reoccuring):</p>
          <form class="don-btn" name="PrePage" method="post" action="https://Simplecheckout.authorize.net/payment/CatalogPayment.aspx"><input type="hidden" name="LinkId" value="e4819acd-b6eb-4f6d-97d6-ca9e2736b685"/><input type="image" src="/assets/images/sky-donate-btn.png"/></form>
      </div>
  </div>
</div>