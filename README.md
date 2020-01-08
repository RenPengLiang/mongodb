## MongoDB数据操作封装说明及范例：

    本文档着重描述如何使用封装的工具类去实现对MongoDB数据的操作

------

###### 后端范例
  
* 在子系统pom.xml中添加公共模块的MongoDB组件pom依赖

  ```java
     <dependency>
       <groupId>com.cjkj</groupId>
       <artifactId>cjkj-mongodb-spring-boot-starter</artifactId>
     </dependency>
  ```

* 访问MongoDB数据时只需要子系统Dao层实现类继承MongoBaseDao即可
  * 使用MongoBaseDao中提供的方法
  * MongoBaseDao中的方法很简单这里就不说明了，就是和操作数据库一样，增删改查api
  
  ```java
   @Component
   public class MongoDao extends MongoBaseDao {  
   }
  ```
