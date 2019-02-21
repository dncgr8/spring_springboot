# spring_springboot
About spring &amp; spring boot basic
## Concepts For knowing spring & spring boot 
 -Beans
 -Annotation
 -Gradle
 -Maven ...


### gradle spring-boot 오류
src/main/resources/application.properties を application.yaml にリネーム
以下の内容を貼り付けると、SpringBootがDB関連のエラーなく起動できるようになる

spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydatabase?mydatabase=true&zeroDateTimeBehavior=convertToNull&autoReconnect=true&useUnicode=true&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone=UTC
    username: mydatabase
    password: mydatabase
    driver-class-name: com.mysql.jdbc.Driver
