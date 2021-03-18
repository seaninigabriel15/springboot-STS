# Spring Tool Suite 4 - Basic Hello World

Using the Spring Tool Suite 4 IDE 

## Spring boot on Spring Tool Suite 4
1. Download Spring Tool Suite 4 (JAR) on https://spring.io/tools
2. Place and paste the jar in your chosen directory 
3. Open the extracted File > Spring Application 
4. Chosose your directory for the project
5. Once open go to File> New > Spring Starter Project
6. Fill the app name > Next > Add Dependencies > WEB/MySQL/Spring Data JPA
7. Under the "src/main/java" create a class SBController.java
8. Paste this :


          package com.springboot.springapp;
          import org.springframework.stereotype.Controller;
          import org.springframework.web.bind.annotation.ResponseBody;
          import org.springframework.web.bind.annotation.RequestMapping;

          @Controller
          public class greetingApp {
            @RequestMapping("/")
            public @ResponseBody String greeting()
            {
              return "Hello World";
            }
          }

9. run and go to browser localhost:8080

If error occured like : 
failed to configure a datasource: 'url' attribute is not specified and no embedded datasource could be configured.

Go to pox.xml and comment the dependency starter data jpa 
## Create Spring boot in Eclipse 
  1.Install Java JDK  

  2.Install Eclipse 

  3.Go to https://start.spring.io/
      Project : Maven
      Langgauge : Java
      Spring boot : 2.4.3
      Group.com.springboot
      artficar/name: spring boot
      
      
  4. Select Dependencies : Web dependecies and Export
  
  5. Eclipse > File > import >Exixting Maven Proj > Select File
  
  6. Create a class file under src/main/java > 
  
  7. Paste this :

              package com.springboot.springapp;
              import org.springframework.stereotype.Controller;
              import org.springframework.web.bind.annotation.ResponseBody;
              import org.springframework.web.bind.annotation.RequestMapping;

              @Controller
              public class greetingApp {

                @RequestMapping("/")
                public @ResponseBody String greeting()
                {
                  return "Hello World";
                }

              }

  6. run on main class
  7. go to localhost:8080 (Tomcat)












