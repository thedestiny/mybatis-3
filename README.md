MyBatis SQL Mapper Framework for Java
=====================================

[![Build Status](https://travis-ci.org/mybatis/mybatis-3.svg?branch=master)](https://travis-ci.org/mybatis/mybatis-3)
[![Coverage Status](https://coveralls.io/repos/mybatis/mybatis-3/badge.svg?branch=master&service=github)](https://coveralls.io/github/mybatis/mybatis-3?branch=master)
[![Maven central](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis)
[![Sonatype Nexus (Snapshots)](https://img.shields.io/nexus/s/https/oss.sonatype.org/org.mybatis/mybatis.svg)](https://oss.sonatype.org/content/repositories/snapshots/org/mybatis/mybatis/)
[![License](http://img.shields.io/:license-apache-brightgreen.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![Stack Overflow](http://img.shields.io/:stack%20overflow-mybatis-brightgreen.svg)](http://stackoverflow.com/questions/tagged/mybatis)
[![Project Stats](https://www.openhub.net/p/mybatis/widgets/project_thin_badge.gif)](https://www.openhub.net/p/mybatis)

![mybatis](http://mybatis.github.io/images/mybatis-logo.png)

The MyBatis SQL mapper framework makes it easier to use a relational database with object-oriented applications.
MyBatis couples objects with stored procedures or SQL statements using a XML descriptor or annotations.
Simplicity is the biggest advantage of the MyBatis data mapper over object relational mapping tools.

Essentials
----------

* [See the docs](http://mybatis.github.io/mybatis-3)
* [Download Latest](https://github.com/mybatis/mybatis-3/releases)
* [Download Snapshot](https://oss.sonatype.org/content/repositories/snapshots/org/mybatis/mybatis/)

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


