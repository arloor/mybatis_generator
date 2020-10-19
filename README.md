## Mybatis generator使用

需要在`insert`或`insertSelective`上加上`useGeneratedKeys="true" keyProperty="id"`

```xml
 <insert id="insertSelective" parameterType="com.xx.xx.xx" useGeneratedKeys="true"
          keyProperty="id">
</insert>
```