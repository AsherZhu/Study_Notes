### Servlet

##### 1. 什么是Servlet?
   * Servlet是sun公司提供的一种用于开发动态web资源的技术。
   * 在API中，Servlet就是一个接口，只需要实现此接口，就可以将此类部署到web服务器中。

##### 2. 编写一个Servlet程序
   1. 写一个java类，实现Servlet接口
   2. 在web.xml中配置Servlet类
   3. 部署项目到Tomcat服务器
   4. 测试http://localhost:8080/Day02_Servlet/demo1 

##### 3. 执行过程

##### 4. Servlet生命周期
实例化→初始化→服务→销毁
* 无参构造方法：服务器创建此类的实例对象时调用
* init():Servlet第一次被访问的时候调用的方法，只会调用一次 
* service():每次访问此类是都会调用此方法
* destroy():销毁Servlet实例调用此方法

#### 5. Servlet的三种创建方式
