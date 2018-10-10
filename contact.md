---
layout: "page"
title: Intranet
permalink: /contact/
---

<style>
      .new-paragraph {
            width: 457px;
      }
      @media only screen and (max-width: 475px) {
            .new-paragraph { 
                  width: 370px;
            }
            .remove-margin-top {
                  margin-top: -200px;
            }
      }
</style>

<section class="page-title parallax-section">
   <div class="row-parallax-bg">
      <div class="parallax-wrapper">
         <div class="parallax-bg">
         <img alt="" src="{{site.baseurl}}/assets/images/bg-image-30.jpg">
      </div>
      </div>
      <div class="parallax-overlay">
      </div>
   </div>
   <div class="centrize">
      <div class="v-center">
         <div class="container">
            <div class="title text-center">
               <!--                <h4 class="upper">Do you need support?</h4>-->
               <h1>Contact Me</h1>
            </div>
         </div>
      </div>
   </div>
</section>
<section class="p-0">
   <div class="container-fluid">
      <div class="row row-flex">
         <div class="col-sm-0"></div>
         <div class="col-sm-6">
            <div class="column-inner with-padding grey-bg">
               <div class="icon-box align-center">
                  <i class="hc-mail-open"></i>
                  <div class="ib-content">
                     <h3>Email</h3>
                     <p><a href="mailto:{{ site.email | encode_email }}">{{ site.email }}</a></p>
                  </div>
               </div>
            </div>
         </div>
         <div class="col-sm-6">
            <div class="column-inner with-padding dark-bg">
               <div class="icon-box align-center">
                  <i class="hc-megaphone"></i>
                  <div class="ib-content">
                     <h3>Call Me</h3>
                     <p>
                        <a href="tel:{{ site.phone }}">
                              {{ site.phone }}
                        </a>
                  </p>
                  </div>
               </div>
            </div>
         </div>
      </div>
   </div>
</section>