# cloud-zipkin

## [zipkin](https://zipkin.io/)

- [GitHub](https://github.com/openzipkin/zipkin)
- [zipkin-server](https://repo1.maven.org/maven2/io/zipkin/java/zipkin-server/)
    - SQL
        ```
        zipkin-server-*.*.*-exec.jar 的 zipkin-storage-mysql-v1-*.*.*.jar 中的 mysql.sql
        ```
    - exec
        ```
        java -jar zipkin-server-*.*.*-exec.jar --STORAGE_TYPE=mysql --MYSQL_HOST=127.0.0.1 --MYSQL_TCP_PORT=3306 --MYSQL_DB=zipkin --MYSQL_USER=root --MYSQL_PASS=root
        ```
