
# 日志链路追踪

程序员蜗牛的日志链路封装SDK

 指定日志配置文件：
``` yaml
 logging:
   config: classpath:logback-spring.xml
```

引入：
```xml
  <dependency>
    <groupId>io.github.foenic.logtrace</groupId>
    <artifactId>logtrace</artifactId>
    <version>1.0</version>
  </dependency>
```

外界排除掉
```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-log4j2</artifactId>
  <version>2.6.7</version>
</dependency>

        <!-- 排除所有默认日志-->
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter</artifactId>
  <exclusions>
    <exclusion>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-logging</artifactId>
    </exclusion>
  </exclusions>
</dependency>
```
