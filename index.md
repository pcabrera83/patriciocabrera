---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekbubyllrb.com/docs/themes/#overriding-theme-defaults

layout: "default"
description: 
permalink: 
---
{% include nav.html %}
<section class="earth-map-bg">
    <div class="container">
        <div class="row pt-50 pb-50">
            <div class="col-md-8 col-md-offset-1">
                <div class="title m-0">
                    <h6 class="capitalize">Hello and Welcome!</h6>
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
<section style="border: none;">
    <div class="container">
        <div class="row">
            <ul id="filters" class="dark-skin">
                {% for tabs in site.data.tabs %}
                <li class="{{ tabs.class }}" data-filter="{{ tabs.data }}">{{ tabs.content }}</li>
                {% endfor %}
            </ul>
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
</section>