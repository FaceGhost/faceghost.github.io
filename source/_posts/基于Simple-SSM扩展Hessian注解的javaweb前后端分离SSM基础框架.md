---
title: 基于Simple-SSM扩展Hessian注解的javaweb前后端分离SSM基础框架
date: 2018-07-24 15:40:32
categories: [ssm]
---

# github地址

 [https://github.com/FaceGhost/Simple-Mult-SSM](https://github.com/FaceGhost/Simple-Mult-SSM "https://github.com/FaceGhost/Simple-Mult-SSM")
 
### 基于Simple-SSM

 [https://github.com/FaceGhost/Simple-SSM](https://github.com/FaceGhost/Simple-SSM "https://github.com/FaceGhost/Simple-SSM")
<!-- more -->
### 开发版本

- jdk1.7 

- spring 4.2.4 

- mybatis 3.2.8 

- hessian 4.0.38

- 开发工具：eclipse

- 数据库：mysql


### 数据库配置文件位置

 [https://github.com/FaceGhost/Simple-Mult-SSM/blob/master/simple-mult-server/src/main/resources/app.properties](https://github.com/FaceGhost/Simple-Mult-SSM/blob/master/simple-mult-server/src/main/resources/app.properties
 "app.properties")

### QuickStart

#### 创建表

```sql 
CREATE TABLE `example` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `user_name` varchar(50) DEFAULT NULL,
  `addr` varchar(500) DEFAULT NULL,
  `sex` tinyint(4) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=3363 DEFAULT CHARSET=utf8;
```  
#### 初始化表数据

```sql 
INSERT INTO `example` VALUES ('3357', '张三', '上海市徐汇区', '1');
INSERT INTO `example` VALUES ('3358', '李四', '北京市朝阳区', '1');
INSERT INTO `example` VALUES ('3359', '王五', '上海金山城市沙滩', '2');
INSERT INTO `example` VALUES ('3360', '麻溜', '上海市长宁区天山路789号', '1');
INSERT INTO `example` VALUES ('3361', '朝七', '上海市嘉定区真南路4500号', '1');
INSERT INTO `example` VALUES ('3362', '黄八', '上海市浦东新区秀浦路798弄之1-7号', '1');
```  

#### 启动

- eclipse 导入

- simple-mult-ssm  项目右键->Debug  As  -> Maven install

- simple-mult-server 项目右键->Debug  As  -> Maven build ...  Goals 输入： tomcat7:run 

- simple-mult-client  项目右键->Debug  As  -> Maven build ...  Goals 输入： tomcat7:run 

### 浏览器访问

 [http://localhost:5000/simple-mult-ssm-client/example](http://localhost:5000/simple-mult-ssm-client/example"simple-mult-ssm-client")

![预览_01](/images/20180724/example_01.png)


#### 关注见鬼网微信公众号，获取有趣文章

![公共号](/images/20180724/faceghost_qc.jpg)

<div id="container"></div>
<link rel="stylesheet" href="https://imsun.github.io/gitment/style/default.css">
<script src="https://imsun.github.io/gitment/dist/gitment.browser.js"></script>
<script>
var gitment = new Gitment({
	id: '201807241540',
  owner: 'FaceGhost',
  repo: 'faceghost.github.io',
  oauth: {
    client_id: 'd227f784f22dc88d715b',
    client_secret: 'e80756438054505e8f1f625430d416dbb2865703',
  },
})
gitment.render('container')
</script>