---
sheetrock_js: >
  <!-- Load Handlebars.js from CloudFlare's CDN. -->
  
  <script src="https://cdnjs.cloudflare.com/ajax/libs/handlebars.js/4.0.5/handlebars.min.js"></script>
  
  <script src="/assets/js/plugins/sheetrock/sheetrock.min.js"></script>
  
  <script lang="javascript">
  var mySpreadsheet = 'https://docs.google.com/spreadsheets/d/12UvjAbdh1OST2unXHNJfRauHnyhwy-FzZVk1cJSnUY0/edit#gid=0';

  $('#vets_helped_count').sheetrock({
    url: mySpreadsheet,
    sql: "select count(A)",
    fetchSize: 0,
  });
  </script>
layout: default
title: "Donate & help honor Veterans with live Taps"
---

<div class="content-container donate">
  <div class="inner-page-banr">
  	<div class="container">
      	<h2>Donate <span>T.A.P.P.S.</span></h2>
      </div>
  </div>
  
  <div class="inner-sections">
  	<div class="container">
  		<div class="top-icon-box">
          	<div style="align: center"><img src="/assets/images/header-top.png" class="header-icon"></div>
          	<div class="top-bx-inner">
              	Your generous donation helps us continue our mission to perform 'Taps' at military funeral performances.
  T.A.P.P.S. is a 501(c) (3) nonprofit organization and all donations are tax deductible. <a href="/assets/501.pdf" target="_blank" style="color:white; text-decoration: underline;">View our 501(c)(3) status letter here.</a>
              </div>
          </div>
          <div class="clearall"></div>
          <div class="donate-sec1">
          	<h4 class="donate-p1"><span>DONATE Today.</span> We need your help. There are many ways to contribute!</h4>
              <p class="donate-p2">T.A.P.P.S. has honored <span id="vets_helped_count"></span> Veterans.  Over 95% of your donation will go to honor their service. How can you help support T.A.P.P.S. Nevada?</p>
              <div class="donate-box">
                <div class="row">
                  <div class="col-sm-12">
                    <div class="card card-price">
                      <div class="card-body">
                        <div class="price" style="line-height: 1em;">STAR WARS TICKETS $15.75/each</div>
                        <div class="lead">Purchase <b>Star Wars: The Rise of Skywalker</b> Fundraiser tickets</div>
                        <ul class="details">
                          <li>Donations are tax deductible.</li>
                        </ul>
                        <form name="PrePage" method="post" action="https://Simplecheckout.authorize.net/payment/CatalogPayment.aspx">
                          <input type="hidden" name="LinkId" value="a78d0821-dd67-4685-81ea-f4df8229cc82"/>
                          <input class="btn btn-primary btn-lg btn-block buy-now" style="font-size: 24px;" type="submit" name="donate_btn" value="BUY TICKETS">
                        </form>
                      </div>
                    </div>
                  </div><!-- /.col -->
                </div>
                <div class="row">


                  <div class="col-sm-4 col-sm-push-4">
                    <div class="card card-price">
                      <div class="card-body">
                        <div class="price">$195</div>
                        <div class="lead">Honor <b>THREE</b> Veterans</div>
                        <ul class="details">
                          <li>Donations are tax deductible.</li>
                        </ul>
                        {% include card-button.html %}
                      </div>
                    </div>
                  </div><!-- /.col -->

                  <div class="col-sm-4 col-sm-pull-4">
                    <div class="card card-price">
                      <div class="card-body">
                        <div class="price">$130</div>
                        <div class="lead">Honor <b>TWO</b> Veterans</div>
                        <ul class="details">
                          <li>Donations are tax deductible.</li>
                        </ul>
                        {% include card-button.html %}
                      </div>
                    </div>
                  </div><!-- /.col -->

                  <div class="col-sm-4">
                    <div class="card card-price">
                      <div class="card-body">
                        <div class="price">$65</div>
                        <div class="lead">Honor <b>ONE</b> Veteran</div>
                        <ul class="details">
                          <li>Donations are tax deductible.</li>
                        </ul>
                        {% include card-button.html %}
                      </div>
                    </div>
                  </div><!-- /.col -->

                </div><!-- /.row -->
              </div><!-- /.donate-box -->
          </div><!-- /.donate-sec1 -->
      </div><!-- /.container -->
  </div><!-- /.inner-sections -->

  <div class="clearall"></div>
  {% include sky-strip.html %}
  <div class="clearall"></div>
  
  <div class="donate-sec-2 amzon-sec">
  	<div class="container">
      <div class="row">
          <div class="col-sm-3">
            <img src="/assets/images/amazon.jpg" alt="amazon" class="img-responsive center-block amazon">
          </div>
          <div class="col-sm-9">
            <p class="amazon-p1">Now when you shop at <span>smile.amazon.com,</span> your purchases will support <br>
    <span>Trumpeters Alliance To Perform Patriotic Services.</span></p>
          </div>
        </div><!-- /.row -->
        <div class="row">
          <div class="col-sm-12">
            <a href="https://smile.amazon.com/" target="_blank"><p class="amazon-p2">Choose T.A.P.P.S. for your charity</p></a>
          </div>
        </div>
      </div><!-- /.container -->
  </div><!-- /.donate-sec-2 -->
  
  <div class="donate-sec-3">
  	<div class="container">
      	<h4 class="strip-heading">T.A.P.P.S. NEVADA would appreciate <br><span>a simple financial contribution.</span></h4>
          <p>Please donate any amount you can here:</p>
          <form class="don-btn" name="PrePage" method="post" action="https://Simplecheckout.authorize.net/payment/CatalogPayment.aspx"><input type="hidden" name="LinkId" value="e4819acd-b6eb-4f6d-97d6-ca9e2736b685"/><input type="image" src="/assets/images/sky-donate-btn.png"/></form>
      </div>
  </div>
</div>