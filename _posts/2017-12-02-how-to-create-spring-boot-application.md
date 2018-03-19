---
layout: post
title:  "How to Create a Spring Boot Application"
date:   2017-12-02
desc: "How to Create a Spring Boot Application"
keywords: "Java,Spring,Boot,gh-pages,website,blog,easy"
categories: [Java]
tags: [Spring,Boot,Spring Boot]
icon: icon-java
---

First, you must go to the following website:
 * [Spring Initializr](https://start.spring.io/)
 
After, fill in the **group** and the **artifact** fields. Example:
 - **Group**: com.mydomain
 - **Artifact**: demo

In the **Search for dependencies** field fill in: **Web**

Another fields can be use the default value. 

After you have filled in all the fields, you will have something corresponding to the image below:

<img src="{{ site.img_path }}/java/first-steps-springboot/start-spring-io.png" width="75%">

Now, click the **Generate Project** button

So, download the ZIP file and unzip it.

Using a text editor ( I recommend [Visual Studio Code] (https://code.visualstudio.com/)), open the demo folder.

Now we are going to create the web controler named HelloWorldController.java:
<img src="{{ site.img_path }}/java/first-steps-springboot/hello-world-controller-java.png" width="75%">

Using the command prompt you can initialize the application using the **mvn spring-boot:run** command using [Maven](https://maven.apache.org).
After the execution you will see the success message referring to the initialization from an embedded Apache Tomcat.

** 2017-12-02 12:40:50.915  INFO 7444 --- [           main] com.example.demo.DemoApplication         : Started DemoApplication in 6.207 seconds (JVM running for
 14.739) **


So, access http://localhost:8080 in the web browser.

<img src="{{ site.img_path }}/java/first-steps-springboot/hello-world-browser-access.png" width="75%"> 

That was pretty easy :)