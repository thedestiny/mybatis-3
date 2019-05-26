#### myabtis 源码笔记

Configuration
XmlConfigBuilder     mybatis-config.xml
XmlMapperBuilder     *Mapper.java
XmlStatementBuilder  *Mapper.xml
XMLScriptBuilder     解析动态sql


mapperRegistry  注册接口的动态代理对象 *mapper.java
loadResources   填充xml文件资源 *mapper.xml
resultMaps 填充resultMap 
sqlFragments 填充sql元素 <sql> 标签内语句
mappedStatements 填充mappedStatements sql 语句
keyGenerators 填充 KeyGenerator 主键自增id


mappedStatement 

```
id -> namespace + id
sqlSource  sql语句
parameterMap 查询参数
resultMaps 返回参数
keyGenerator  useGeneratedKeys=true keyProperty=id

```


BaseJdbcLogger

ConnectionLogger -> PreparedStatementLogger -> ResultSetLogger -> StatementLogger

InvocationHandler


MetaObject

objectFactory
objectWrapperFactory
reflectorFactory


