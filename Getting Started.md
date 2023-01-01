## 1. System Requirements 
● Java 8  
● Maven 3.3+  
● idea 2022
## 2. HelloWorld Application  
Requirements: send /hello request, server response "hello spring boot2"
### 2.1 Create project
Create a maven project in IDEA 
### 2.2 Creating the POM, add dependencies
```xml
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>3.0.1</version>
</parent>

<dependencies>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>
</dependencies>
```
### 2.3 Creating the Main Class
```java
/**
 * Main Class
 * @SpringBootApplication：the annotation shows this is a SpringBoot Application
 */
@SpringBootApplication
public class MainApplication {

    public static void main(String[] args) {
        SpringApplication.run(MainApplication.class,args);
    }
}
```
### 2.4 Adding Controller
```java
@RestController
public class HelloController {
    @RequestMapping("/hello")
    public String handle01(){
        return "Hello, Spring Boot 2!";
    }
}
```
### 2.5 Test
Running the Example, in browser open localhost:8080\hello
### 2.6 Simplifying configurations
Create a file "application.properties" in "src\main\resources"  
E.G. Change listening port from default 8080 to 8888
```
server.port=8888 
```
Visit full documentation -- https://docs.spring.io/spring-boot/docs/current/reference/html/application-properties.html#appendix.application-properties.core


