## Mybatis generator使用

### 用法

```shell
mvn -Dmybatis.generator.overwrite=true mybatis-generator:generate
```

```shell
mvn mybatis-generator:generate
```


### 主键生成 

需要在`insert`或`insertSelective`上加上`useGeneratedKeys="true" keyProperty="id"`

```xml
 <insert id="insertSelective" parameterType="com.xx.xx.xx" useGeneratedKeys="true"
          keyProperty="id">
</insert>
```