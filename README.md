# cloud-zipkin

## [zipkin](https://zipkin.io/)

- [GitHub](https://github.com/openzipkin/zipkin)
- [zipkin-server](https://repo1.maven.org/maven2/io/zipkin/java/zipkin-server/)
    - 端口
        - 9411
            - 前端页面端口
        - 9092
            - 接收Kafka等参数端口
    - SQL
        ```
        zipkin-server-*.*.*-exec.jar 中的 zipkin-storage-mysql-v1-*.*.*.jar 中的 mysql.sql
        ```
    - exec
        - MySQL 数据库密码插件`mysql_native_password`
        ```
        java -jar zipkin-server-*.*.*-exec.jar --STORAGE_TYPE=mysql --MYSQL_HOST=127.0.0.1 --MYSQL_TCP_PORT=3306 --MYSQL_DB=zipkin --MYSQL_USER=root --MYSQL_PASS=root
        ```
        - Kafka
        ```
        java -jar zipkin-server-*.*.*-exec.jar --KAFKA_BOOTSTRAP_SERVERS=127.0.0.1:9092
        ```
