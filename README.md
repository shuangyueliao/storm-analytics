这个例子的功能是统计浏览了某个产品的用户还浏览了哪类产品
[代码连接](https://github.com/shuangyueliao/storm-analytics)

1. 运行类TopologyStarter的main方法，启动后台统计功能，注意redis要启动
2. 运行页面展示模块node webapp/app.js 
3. 访问地址http://localhost:3000/

部分页面展示：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201127171800336.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NodWFuZ3l1ZWxpYW8=,size_16,color_FFFFFF,t_70)
这个例子中有三个主要组件

 - 基于node.js的web应用
 - redis服务器，用于持久化数据
 - 一个storm拓扑，用于分布式实时处理数据

 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20201127223553281.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3NodWFuZ3l1ZWxpYW8=,size_16,color_FFFFFF,t_70)
