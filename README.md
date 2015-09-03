# mybatis-maven-generator
基于maven的mybatis/ibatis的代码生成器

# 使用
src/resources/generatorConfig.xml : 修改配置 jdbcConnection, jdbc-url, user/password 

# 执行
mvn compile exec:java

# 注意
新增特性：
	* 中文注释
	* `context.targetRuntime=IbatisJava5 && javaClientGenerator.type=SPRING` 场景下，新增2个可选propery: `superClass && annotation` 用于自定义 DAOImpl的父类和注解