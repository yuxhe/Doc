# H2

表示可以在浏览器中访问H2的控制台

- spring.h2.console.enabled=true

然后以java application运行，运行之后在浏览器中访问localhost:8080/h2-console即可进入h2配置页面，可以选择语言为中文。

### 报错以及解决方案

```
Parameter 0 of constructor in org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaAutoConfiguration required a bean of type 'javax.sql.DataSource' that could not be found.
    - Bean method 'dataSource' not loaded because @ConditionalOnClass did not find required class 'org.springframework.jdbc.datasource.embedded.EmbeddedDatabaseType'
    - Bean method 'dataSource' not loaded because @ConditionalOnClass did not find required class 'org.springframework.jdbc.datasource.embedded.EmbeddedDatabaseType'

```

#### 解决方案

1. 查看 effiect pom ,搜索spring-jdbc, 查看其版本号
2. 进入maven 本地仓库,删除 ```org.springframework.spring-jdbc```下该版本号的内容
3. Reimport/update maven dependency



