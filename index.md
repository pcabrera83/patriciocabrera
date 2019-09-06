---
layout: "page"
title: "Homepage"
description:
permalink:
---

<section class="earth-map-bg">
    <div class="container">
        <div class="row pt-50 pb-50">
            <div class="col-md-8 col-md-offset-1">
                <div class="title m-0">
                    <h4 class="upper">Hello and Welcome!</h4>
                    <h1 class="fw-400">I am a UX Designer who likes to create cool <span class="typed-words fw-600 colored-text"
                            data-strings="[&quot;apps&quot;, &quot;websites&quot;, &quot;software&quot;]"></span>that
                        people enjoy using.</h1>
                </div>
            </div>
        </div>
    </div>
</section>
<!-- 
    Project Section 
-->
<section class="gradient-bg section-skewed big-padding-bt" data-gradients="#00c3da,#07B5DE" style="border: none;">
    <div class="gradient-bg-wrapper">
        <div class="gradient-bg-element" style="background: rgba(0, 0, 0, 0) linear-gradient(90deg, rgb(255, 121, 95) 0%, rgb(206, 23, 104) 100%) repeat scroll 0% 0%;"></div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-md-5">
                <div class="title txt-sm-center">
                    <h4 class="upper">what I do</h4>
                    <h2>Selected Works</h2>
                </div>
            </div>
            <div class="col-md-6 col-md-offset-1">
                <ul id="filters" class="mt-50">
                    {% for tabs in site.data.tabs %}
                    <li class="{{ tabs.class }}" data-filter="{{ tabs.data }}">{{ tabs.content }}</li>
                    {% endfor %}
                </ul>
            </div>
            <div class="skewed-mask">
                <div class="mask-block" style="background: rgb(247, 247, 247) none repeat scroll 0% 0%;">
                </div>
            </div>
        </div>
    </div>
</section>
<section class="grey-bg section-skewed pt-0">
    <div class="container">
        <div class="row" data-negative-margin="150" style="margin-top: -150px;">
            <div id="works-grid" class="four-col with-spacing">
                {% for project in site.data.project %}
                <a href="{{ project.url | relative_url }}">
                    <div class="work-item {{ project.class }}">
                        <div class="work-detail">
                            <img src="{{ project.imgSrc | relative_url }}" alt="{{ project.imgAlt }}">
                            <div class="work-info">
                                <div class="centrize">
                                    <div class="v-center">
                                        <h3>{{ project.title }}</h3>
                                        <p>{{ project.description }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </a>
                {% endfor %}
            </div>
        </div>
    </div>
    <div class="skewed-mask">
        <div class="mask-block" style="background: rgb(255, 255, 255) none repeat scroll 0% 0%;">
        </div>
    </div>
</section>
<!-- Expertise Section -->
<section class="dark-bg section-skewed">
    <div class="container">
        <div class="title">
            <h2>Experience</h2>
            <p class="fw-300">
                As a UX Designer, I’ve been extremely successful in achieving results in the areas of user-centered
                design, website/app design, and front-end development for many different types of business from
                non-profits, consulting, eCommerce and B2B.
            </p>
        </div>
        <div class="section-content pt-25 pb-25">
            <div class="row">
                <div class="col-md-3 col-sm-6">
                    <div class="icon-box animated fadeInRight" data-animation="fadeInRight">
                        <div class="animated-icon white" data-icon="images/icons/paintroller.svg"><svg version="1.0" id="Layer_1"
                                xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                                width="100%" height="100%" viewBox="0 0 64 64" enable-background="new 0 0 64 64"
                                xml:space="preserve">
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" width="48"
                                    height="17" d="M7 1 L55 1 L55 18 L7 18 Z" style="stroke-dasharray: 130, 132; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M2,9L7,9"
                                    style="stroke-dasharray: 5, 7; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M55,9L61,9L61,24L32,24L32,41"
                                    style="stroke-dasharray: 67, 69; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" width="8"
                                    height="21" d="M28 42 L36 42 L36 63 L28 63 Z" style="stroke-dasharray: 58, 60; stroke-dashoffset: 0;"></path>
                            </svg></div>
                        <div class="ib-content">
                            <h4 class="upper">Branding</h4>
                            <ul class="list-unstyled">
                                <li>Logos</li>
                                <li>Corporate Identity</li>
                                <li>Business Cards</li>
                                <li>Packaging</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6">
                    <div class="icon-box animated fadeInRight" data-animation="fadeInRight" data-delay="300">
                        <div class="animated-icon white" data-icon="images/icons/server.svg"><svg version="1.1" id="Layer_1"
                                xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                                width="100%" height="100%" viewBox="0 0 64 64" enable-background="new 0 0 64 64"
                                xml:space="preserve">
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M59,56  c0,3.866-11.641,7-26,7S7,59.866,7,56" style="stroke-dasharray: 57, 59; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M59,40  c0,3.866-11.641,7-26,7S7,43.866,7,40" style="stroke-dasharray: 57, 59; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M59,24  c0,3.866-11.641,7-26,7S7,27.866,7,24" style="stroke-dasharray: 57, 59; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M7,8A26,7 0,1,1 59,8A26,7 0,1,1 7,8" style="stroke-dasharray: 113, 115; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M7,8L7,56" style="stroke-dasharray: 48, 50; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M59,8L59,56" style="stroke-dasharray: 48, 50; stroke-dashoffset: 0;"></path>
                            </svg></div>
                        <div class="ib-content">
                            <h4 class="upper">Development</h4>
                            <ul class="list-unstyled">
                                <li>Websites</li>
                                <li>Native Apps</li>
                                <li>WordPress</li>
                                <li>eCommerce</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6">
                    <div class="icon-box animated fadeInRight" data-animation="fadeInRight" data-delay="600">
                        <div class="animated-icon white" data-icon="images/icons/compass.svg"><svg version="1.1" id="Layer_1"
                                xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                                width="100%" height="100%" viewBox="0 0 64 64" enable-background="new 0 0 64 64"
                                xml:space="preserve">
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M3.7079999999999984,35A28.292,28.292 0,1,1 60.292,35A28.292,28.292 0,1,1 3.7079999999999984,35"
                                    style="stroke-dasharray: 178, 180; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-linejoin="bevel"
                                    stroke-miterlimit="10" d="M37,40L45,21L26,29L19,47Z" style="stroke-dasharray: 80, 82; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M26,29L37,40"
                                    style="stroke-dasharray: 16, 18; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M36.9,7C36.965,6.677,37,6.342,37,6  c0-2.761-2.239-5-5-5s-5,2.239-5,5c0,0.342,0.035,0.677,0.1,1"
                                    style="stroke-dasharray: 18, 20; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M32,7L32,12"
                                    style="stroke-dasharray: 5, 7; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M32,58L32,63"
                                    style="stroke-dasharray: 5, 7; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M60,35L55,35"
                                    style="stroke-dasharray: 5, 7; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M9,35L4,35"
                                    style="stroke-dasharray: 5, 7; stroke-dashoffset: 0;"></path>
                            </svg></div>
                        <div class="ib-content">
                            <h4 class="upper">Marketing</h4>
                            <ul class="list-unstyled">
                                <li>Strategy</li>
                                <li>SEO</li>
                                <li>Sales</li>
                                <li>Email Campaigns</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6">
                    <div class="icon-box animated fadeInRight" data-animation="fadeInRight" data-delay="900">
                        <div class="animated-icon white" data-icon="images/icons/cards-diamonds.svg"><svg version="1.1"
                                id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                                x="0px" y="0px" width="100%" height="100%" viewBox="0 0 64 64" enable-background="new 0 0 64 64"
                                xml:space="preserve">
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M44,59L16,45L36,5L63,19Z"
                                    style="stroke-dasharray: 151, 153; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M31.899,14.004L28,6L1,20L19,59L32,52.964"
                                    style="stroke-dasharray: 97, 99; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M35,41L46,36L45,24L34,29Z"
                                    style="stroke-dasharray: 49, 51; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M38,9L37,11"
                                    style="stroke-dasharray: 3, 5; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M7,23L6,21"
                                    style="stroke-dasharray: 3, 5; stroke-dashoffset: 0;"></path>
                                <path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M43,53L42,55"
                                    style="stroke-dasharray: 3, 5; stroke-dashoffset: 0;"></path>
                            </svg></div>
                        <div class="ib-content">
                            <h4 class="upper">Product Design</h4>
                            <ul class="list-unstyled">
                                <li>UX App Design</li>
                                <li>Corporate Identity</li>
                                <li>Business Cards</li>
                                <li>Packaging</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="skewed-mask">
        <div class="mask-block" style="background: rgb(247, 247, 247) none repeat scroll 0% 0%;"></div>
    </div>
</section>