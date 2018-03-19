---
layout: post
title:  "How to Create a Spring Boot Application using Kotlin and Gradle"
date:   2018-03-10
desc: "How to Create a Spring Boot Application using Kotlin and Gradle"
keywords: "Kotlin,Java,Spring,Boot,gh-pages,website,blog,easy"
categories: [Kotlin]
tags: [Spring,Boot,Spring Boot,Kotlin]
icon: icon-java
---

A few months ago I wrote an article showing how to create a simple Spring Boot application using Java, you can see it [clicking here](https://thiagoteixeira.github.io/java/2017/12/02/how-to-create-spring-boot-application.html).

Now, I am going to show you, how to create the same application using [Kotlin](https://kotlinlang.org/) and [Gradle](https://gradle.org/) installed.

The requirements are:
 - [Gradle](https://gradle.org/) installed;
 - Text Editor installed, I recommend [Visual Studio Code] (https://code.visualstudio.com/)
 

Now, you must go to the following website:
 * [Spring Initializr](https://start.spring.io/)
 
Choose to generate a **Gradle Project** with **Kotlin** and fill in the **group** and the **artifact** fields. Example:
 - **Group**: com.mydomain
 - **Artifact**: demo
 
In the **Search for dependencies** field fill in: **Web**

The options chosen will be as the image below:

<img src="{{ site.img_path }}/kotlin/how-to-create-spring-boot-with-kotlin-and-gradle/spring-initializr-options-chosen.png" width="75%">

Now, click the **Generate Project** button

So, download the ZIP file and unzip it.

Using a text editor ( I recommend [Visual Studio Code](https://code.visualstudio.com/)), open the demo folder.

Now we are going to create the web controler file named HelloWorldController.kt at **demo\src\main\kotlin\com\example\demo\** folder:

<img src="{{ site.img_path }}/kotlin/how-to-create-spring-boot-with-kotlin-and-gradle/hello-world-controller-file.png" width="50%">

Your respective code will be:

```
package com.example.demo

import org.springframework.web.bind.annotation.GetMapping
import org.springframework.web.bind.annotation.RestController

@RestController
class HelloWorldController {

    @GetMapping("/")
    fun index() = "Hello, World!"

}
```

Now, using the command prompt you can initialize the application using the **gradle bootrun** command using [Gradle](https://gradle.org/).
After the execution you will see the success message referring to the initialization from an embedded Apache Tomcat.

**
<==========---> 80% EXECUTING [1m 40s]
> :bootRun **
**

So, access http://localhost:8080 in the web browser.

<img src="{{ site.img_path }}/kotlin/how-to-create-spring-boot-with-kotlin-and-gradle/hello-world-browser-access.png" width="75%">

Finally, your first Spring Boot application with Kotlin and Gradle was created.

Thanks for reading.