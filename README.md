# mybatis-generator-repository-annotation-plugin

add repository annotation to generation object ，like this

```java
@Repository
public interface AccountMapper {
    
}
```

## why?

if has not this annotation, idea should show error ,you can see https://stackoverflow.com/questions/25379348/idea-inspects-batis-mapper-bean-wrong

## install

add this to mvn file 
```xml
<pluginRepositories>
	<pluginRepository>
		<id>mybatis-generator-repository-annotation-plugin</id>
		<url>https://raw.github.com/zgj1024/mybatis-generator-repository-annotation-plugin/mvn-repo/</url>
	</pluginRepository>
</pluginRepositories>
```

add this dependency
```xml
<dependency>
	<groupId>com.zgj</groupId>
	<artifactId>mybatis-generator-repository-annotation-plugin</artifactId>
	<version>1.0.0</version>
</dependency>
```

## use

add plugin to mybatis generation file  

```xml
<plugin type="com.zgj.mybatis.plugins.RepositoryAnnotationPlugin" />
```