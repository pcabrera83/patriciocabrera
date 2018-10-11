---
layout: "post"
title: "About Me"
description:
author: Patricio Cabrera
date: October 11, 2018
category: Biography
permalink: /about
---
<style>
    p {
        color: #787878;
        font-size: 16px;
    }
</style>   
<section class="page-title parallax-section">
    <div class="row-parallax-bg">
        <div class="parallax-wrapper">
            <div class="parallax-bg">
                <img src="{{ site.baseurl }}/assets/images/cuenca.jpeg" alt="">
            </div>
        </div>
        <div class="parallax-overlay"></div>
    </div>
    <div class="centrize">
        <div class="v-center">
            <div class="container">
                <div class="single-post-info">
                <div class="title text-center">
                    <h1 style="font-weight: 700;">{{ page.title }}</h1>
                </div>
                    <div class="post-author">
                        <img style="width: 140px;" src="{{ site.baseurl }}/assets/images/patricio-headshot.jpg" alt="">
                        <!-- <a href="#"> 
                        by {{ page.author}}
                        </a> -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
<section>
        <div class="container">
          <div class="row">
            <div class="col-md-8 col-md-offset-2">
              <article class="post-single">
                <div class="post-body">
                  <p class="first-letter">This is the <strong>about me page</strong>. What to say? Like many of you, I struggle with talking about myself, which in my line of work is not good. We can start at what I do, as you probably guessed, I am a UX/UI designer based in the Northeast of the U.S.A.
                  </p>
                  <p>I love my work and I constantly looking at new ways to innovate and challenge myself. Which reminds me of this qoute by Henry Ford.</p>
                  <blockquote>
                    <p>If I had asked people what they wanted, they would have said faster horses.</p>
                  </blockquote>
                  <img src="{{ site.baseurl }}/assets/images/riocuenca.jpg" alt="" data-action="zoom">
                  <p>When I'm not at work, you can find me at home spending time with my wife and kids. Watching movies, cycling, running or playing video games.</p>
                  <p>Oh the pictures on this page are from my hometown of Cuenca, Ecuador. I love the architeture and I feel people don't know about it. So why not show my hometown some love.</p>
                  <h3 style="font-weight: 700; font-family: 'Poppins', sans-serif; color: #1f1f1f; line-height: 1.3;     font-size: 24px;}">Fun Facts</h3>
                  <ul>
                  {% for facts in site.data.facts %}
                    <li>{{ facts.name}}</li>
                    {% endfor %}
                  </ul>
                </div>
                <!-- <div class="tagcloud">
                    {% for skills in site.data.skills %}
                    <a href="{{ skills.link }}">{{skills.content}}</a>
                    {% endfor %}
                </div> -->
              </article>
            </div>
          </div>
        </div>
      </section>