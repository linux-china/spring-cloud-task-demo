Spring Cloud Task
=================
Spring Cloud Task就是执行一个短的任务，也就是启动JVM进程执行，然后退出程序，
将执行任务的结果记录下来。

### 使用

* 首先你要创建一个数据库来记录task执行情况
* 创建一个Spring Boot应用，然后创建一个CommandLineRunner的Bean
* 执行 mvn -DskipTests clean package会调用Spring Boot Maven plugin，生成一个fat jar
* 提交fat jar到执行平台执行即可

### 注意

* 和Cron不一样，那个驻留定时执行
