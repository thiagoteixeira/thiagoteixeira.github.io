---
layout: post
title: How to Create a Spring Boot Application
author: thiago
date: 2017-12-02 13:32:20 +0300
description: How to Create a Spring Boot Application. # Add post description (optional)
image: assets/images/spring/spring-boot-20171202.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Java,Spring,Boot,blog]
categories: [ tutorial ]
---

First, you must go to the following website:
 * [Spring Initializr](https://start.spring.io/)
 
After, fill in the **group** and the **artifact** fields. Example:
 - **Group**: com.mydomain
 - **Artifact**: demo

In the **Search for dependencies** field fill in: **Web**

The other fields can use the default value. 

After you have filled in all the fields, you will have something corresponding to the image below:

![First step with Sprint Boot]({{site.baseurl}}/assets/images/java/first-steps-springboot/start-spring-io.png)

Now, click on the **Generate Project** button

So, download the ZIP file and unzip it.

Using a text editor ( I recommend [Visual Studio Code](https://code.visualstudio.com/)), open the demo folder.

Now we are going to create the web controller named HelloWorldController.java:
![Hello World Controller using Spring Boot]({{site.baseurl}}/assets/images/java/first-steps-springboot/hello-world-controller-java.png)

Using the command prompt you can initialize the application using the **mvn spring-boot:run** command using [Maven](https://maven.apache.org).
After the execution, you will see the success message referring to the initialization from an embedded Apache Tomcat.

** 2017-12-02 12:40:50.915  INFO 7444 --- [           main] com.example.demo.DemoApplication         : Started DemoApplication in 6.207 seconds (JVM running for
 14.739) **

So, access http://localhost:8080 in the web browser.

![Hello World Controller using Spring Boot in the browser]({{site.baseurl}}/assets/images/java/first-steps-springboot/hello-world-browser-access.png)

That was pretty easy :)