---
layout: page
title: Developer, Blogger, Speaker, Teacher and Husband.
permalink: /about
comments: true
---
<div class="row justify-content-between pt-4">
<div class="col-md-8 pr-5">
            <section class="featured-posts pb-3">
                <div class="row">
                    <div class="col-md-4 text-center pb-sm-5">
                        <div class="profile-pic">                            
                            <div class="flip-card-inner">
                                <div class="flip-card-front">
                                <img class="lozad" src="{{site.baseurl}}/assets/images/thiagoteixeira-profile.png" alt="Thiago Teixeira"></div>
                                <div class="flip-card-back">
                                <img class="lozad" src="{{site.baseurl}}/assets/images/thiagoteixeira-profile-2.png" alt="Thiago Teixeira"></div>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <p></p>
                        <ul>
                            <li>Senior Software Engineer at <a href="https://ciandt.com/" target="_blank">CI&T</a></li>
                            <li>Open-source software aficionado and a technology advocate by passion &
                                profession</li>                                                        
                            <li>Cloud & Container technology enthusiast and advocate</li>
                            <li>Passionate about developer experience and user experience</li>
                            <li>Certifications:</li>
                            <div class="col">
                                <p></p>
                                <ul>
                                    <li><a href="https://www.youracclaim.com/org/oracle/badge/oracle-certified-expert-java-ee-6-enterprise-javabeans-developer" target="_blank">Oracle Certified Expert, Java EE 6 Enterprise JavaBeans</a></li>
                                    <li><a href="https://www.youracclaim.com/badges/05beea07-9bd3-4f28-9fc0-59e98952525d" target="_blank">Oracle Certified Expert, Java EE 6 Web Component Developer</a></li>
                                    <li><a href="https://www.youracclaim.com/org/oracle/badge/oracle-certified-professional-java-se-6-programmer" target="_blank">Oracle Certified Professional, Java SE 6 Programmer</a></li>
                                </ul>
                                <p></p>
                            </div>
                        </ul>
                        <p></p>
                    </div>
                </div>
            </section>
        </div>
        <div class="col-md-4">
            <div class="sticky-top sticky-top-80">
                <section class="featured-posts">
                    <div class="section-title">
                        <h2><span>Follow me on social media</span></h2>
                    </div>
                    <div class="about-social">
                        <a href="https://twitter.com/teixeira_thi"><i class="fab fa-twitter fa-lg"></i> </a>                                
                        <a href="https://www.linkedin.com/in/thiagoaugustoteixeira"><i class="fab fa-linkedin fa-lg"></i></a>
                        <a href="https://medium.com/@teixeirathiago"><i class="fab fa-medium fa-lg"></i></a>                        
                        <a href="https://github.com/thiagoteixeira"><i class="fab fa-github fa-lg"></i></a>
                    </div>
                </section>
                <section>
                    <div class="section-title">
                        <h2><span>Blogs on Dev.to</span></h2>
                    </div>
                    <dev-widget data-username="thiagoteixeira" data-width="100%"></dev-widget>
                </section>
                <!--
                <div class="ad-holder w-100 mb-3">
                    <script async type="text/javascript"
                        src="//cdn.carbonads.com/carbon.js?serve=CE7ITK3I&placement=thiagoteixeira"
                        id="_carbonads_js"></script>
                </div>
                <section class="featured-posts">
                    <div class="section-title">
                        <h2><span>Upcoming talks</span></h2>
                    </div>
                    <div class="row"></div>
                </section>
                -->
                <section class="featured-posts">
                    <div class="section-title">
                        <h2><span>Featured</span></h2>
                    </div>
                    <div class="row">
                    {% for post in site.posts %}
                        {% if post.featured == true %}
                            {% include featuredbox_row.html %}
                        {% endif %}
                    {% endfor %}
                    </div>
                </section>
            </div>
        </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/lozad.js/1.14.0/lozad.min.js"
        integrity="sha256-hstwhDmGVwZjIwt6SlTG6sQBREWrWTBjVTik/JLlb1Y=" crossorigin="anonymous"></script>
    <script async src="https://unpkg.com/dev-widget@1.1.0/dist/card.component.min.mjs" type="module"></script>

</div>
