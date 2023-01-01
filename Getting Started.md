## 1. System Requirements 
● Java 8  
● Maven 3.3+  
● idea 2022
## 2. HelloWorld Application  
Requirements: send /hello request, server response "hello spring boot2"
### 2.1 Create a maven project in IDEA
### 2.2 Creating the POM
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
