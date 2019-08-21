# 引入Maven依赖

引入下面的依赖
```xml
    <dependency>
        <groupId>com.chinasofti.futurelab.event</groupId>
        <artifactId>rabbit</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>
```

删除spring的自动配置
```java
@SpringBootApplication(exclude = {RabbitAutoConfiguration.class})
public class MiddleApplication {
    public static void main(String[] args) {
        SpringApplication.run(MiddleApplication.class, args);
    }
}
```
