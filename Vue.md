#### VUE

##### 1，Declarative Rendering





#### Quasar



#### 微服务

​	微服务架构风格是将every single APP的角色视作为a suite of small services，这些single APP服务都在其自己的进程中运行，并以HTTP进行通信。

​	相对于微服务风格（Micro-service Style）的是整体服务（Monolithic Style）；整体服务架构的APP是建立在三个主要部分：客户端、数据库、服务端；服务端负责处理HTTP请求，执行特定领域逻辑，通过数据库进行检索和更新数据，返回数据给客户端。整体风格有一个缺陷在于：系统的任何更改都会涉及重新构建和部署。

​	Micro-services provide benefits:

+ 服务组件化(Componentization via services)

  组件(Component)指的是，a unit of software that is independently replaceable and upgradeable.

  + Library和service的区别

  ​	微服务架构会用到libraries，libraries被视作components，并且会被程序引用（引用是发生在进程内）。

  ​	services也同样被视作components，但是它们分属不同的进程。services之间的通信是通过web请求或者远程调用来实现的。

  https://www.martinfowler.com/articles/microservices.html

+ 