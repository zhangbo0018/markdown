# mall项目架构及功能概览
                mall项目架构及功能概览                   

💡 快速上手

mall项目架构及功能概览

mall项目架构及功能概览
=============

返回文档

本节课程作为《mall学习教程》的开篇，主要对mall项目中使用的技术、功能及数据库表进行介绍，希望大家能对mall项目有所了解。  
  
mall项目简介  
  
mall项目是一套电商系统，包括前台商城系统及后台管理系统，基于SpringBoot+MyBatis实现。前台商城系统包含首页门户、商品推荐、商品搜索、商品展示、购物车、订单流程、会员中心、客户服务、帮助中心等模块。 后台管理系统包含商品管理、订单管理、会员管理、促销管理、运营管理、内容管理、统计报表、财务管理、权限管理、设置等模块。  
  
项目演示  
  
后台管理系统  
  
后台管理系统演示地址：[https://www.macrozheng.com/admin/index.html](https://www.macrozheng.com/admin/index.html)  
  

![](https://www.yuque.com/api/filetransfer/images?url=https%3A%2F%2Fmacro-oss.oss-cn-shenzhen.aliyuncs.com%2Fmall%2Fteach%2Fre_mall_foreword_01.png%3Fx-oss-process%3Dimage%252Fwatermark%252Ctype_d3F5LW1pY3JvaGVp%252Csize_42%252Ctext_5YWs5LyX5Y-377yabWFjcm96aGVuZw%253D%253D%252Ccolor_FFFFFF%252Cshadow_50%252Ct_80%252Cg_se%252Cx_10%252Cy_10&sign=c2dae4de83ec0b0f5f75d88c0fb7b3e770e69bf2a1293f2ae801bba69f0f27ca)

  
  
移动端商城  
  
移动端商城演示：[https://www.macrozheng.com/app/index.html](https://www.macrozheng.com/app/mainpage.html)  
  

![](https://www.yuque.com/api/filetransfer/images?url=https%3A%2F%2Fmacro-oss.oss-cn-shenzhen.aliyuncs.com%2Fmall%2Fteach%2Fre_mall_foreword_08.jpg%3Fx-oss-process%3Dimage%252Fwatermark%252Ctype_d3F5LW1pY3JvaGVp%252Csize_33%252Ctext_5YWs5LyX5Y-377yabWFjcm96aGVuZw%253D%253D%252Ccolor_FFFFFF%252Cshadow_50%252Ct_80%252Cg_se%252Cx_10%252Cy_10&sign=5b5738dc6848f821749f3da31c3a91ae8c3af57dde703ed88f795e00df034333)

  
  
mall中使用的技术  
  
后端技术  
  
mall采用现阶主流技术实现，涵盖了一般项目中几乎所有使用的技术。  
| 

技术  

 | 

版本  

 | 

说明  

 |
| 

SpringBoot  

 | 

2.7.5  

 | 

容器+MVC框架  

 |
| 

SpringSecurity  

 | 

5.7.4  

 | 

认证和授权框架  

 |
| 

MyBatis  

 | 

3.5.10  

 | 

ORM框架  

 |
| 

MyBatisGenerator  

 | 

1.4.1  

 | 

数据层代码生成  

 |
| 

RabbitMQ  

 | 

3.10.5  

 | 

消息队列  

 |
| 

Redis  

 | 

7.0  

 | 

分布式缓存  

 |
| 

MongoDB  

 | 

5.0  

 | 

NoSql数据库  

 |
| 

Elasticsearch  

 | 

7.17.3  

 | 

搜索引擎  

 |
| 

LogStash  

 | 

7.17.3  

 | 

日志收集工具  

 |
| 

Kibana  

 | 

7.17.3  

 | 

日志可视化查看工具  

 |
| 

Nginx  

 | 

1.22  

 | 

静态资源服务器  

 |
| 

Druid  

 | 

1.2.14  

 | 

数据库连接池  

 |
| 

MinIO  

 | 

8.4.5  

 | 

对象存储  

 |
| 

Hutool  

 | 

5.8.0  

 | 

Java工具类库  

 |
| 

PageHelper  

 | 

5.3.2  

 | 

MyBatis物理分页插件  

 |
| 

Swagger-UI  

 | 

3.0.0  

 | 

文档生成工具  

 |
| 

logstash-logback-encoder  

 | 

7.2  

 | 

Logstash日志收集插件  

 |
| 

docker-maven-plugin  

 | 

0.40.2  

 | 

应用打包成Docker镜像的Maven插件  

 |  
前端技术  
  
mall项目采用现阶段流行的前后端分离开发模式，mall-admin-web作为电商管理系统的前端项目，基于Vue+Element实现。  
| 

技术  

 | 

说明  

 |
| 

Vue  

 | 

前端框架  

 |
| 

Vue-router  

 | 

路由框架  

 |
| 

Vuex  

 | 

全局状态管理框架  

 |
| 

Element  

 | 

前端UI框架  

 |
| 

Axios  

 | 

前端HTTP框架  

 |
| 

v-charts  

 | 

基于Echarts的图表框架  

 |
| 

Js-cookie  

 | 

cookie管理工具  

 |
| 

nprogress  

 | 

进度条控件  

 |
| 

vue-element-admin  

 | 

项目脚手架参考  

 |  
移动端技术  
  
mall-app-web作为电商系统的移动端项目，基于uni-app实现。主要包括首页门户、商品推荐、商品搜索、商品展示、购物车、订单流程、会员中心、客户服务、帮助中心等功能。  
| 

技术  

 | 

说明  

 |
| 

Vue  

 | 

核心前端框架  

 |
| 

Vuex  

 | 

全局状态管理框架  

 |
| 

uni-app  

 | 

移动端前端框架  

 |
| 

mix-mall  

 | 

电商项目模板  

 |
| 

luch-request  

 | 

HTTP请求框架  

 |mall实现的功能概览  
后台管理系统  
  
mall项目的后台管理系统，主要分为商品模块、订单模块、营销模块和权限模块，目前来说已经比较完善了，足以支撑一套完整的电商流程。  
  
●商品模块包括：商品管理、商品分类管理、商品类型管理、品牌管理  
  
  
●订单模块包括：订单管理、订单设置、退货申请处理、退货原因设置  
  
  
●营销模块包括：秒杀活动管理、优惠券管理、品牌推荐管理、新品推荐管理、人气推荐管理、专题推荐管理、首页广告管理  
  
  
●权限模块包括：用户管理、菜单管理、角色管理、资源管理  
  
  
移动端商城  
  
移动端商城目前已经可以实现完整的电商流程，具体功能可参考下图。  
  
  
mall数据库表概览  
  
mall项目目前有76张数据表，业务逻辑有一定复杂度，平时做项目参考也够了。  
  

  
  
数据库表前缀说明  
  
●pms\_\*：商品模块相关表  
●oms\_\*：订单模块相关表  
●sms\_\*：营销模块相关表  
●ums\_\*：权限模块相关表  
●cms\_\*：内容模块相关表  

​

13 人点赞

*   ![](https://cdn.nlark.com/yuque/0/2022/png/23033879/1655352430694-avatar/7374fa21-f544-44a7-8991-1e9cda15226d.png?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*khrYRYi6VN0AAAAAAAAAAAAADvuFAQ/original)
    
*   ![](https://cdn.nlark.com/yuque/0/2022/png/22164601/1662172629309-avatar/a736f8fd-c8dd-4368-93e1-b7e783b1e3bb.png?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://cdn.nlark.com/yuque/0/2023/jpeg/anonymous/1678182093393-333023a8-e1c0-453e-acc8-3520b5bbf1ea.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://cdn.nlark.com/yuque/0/2022/jpeg/anonymous/1648279916193-8cabefd8-85a6-4cbc-9255-afdfd4f12e31.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://cdn.nlark.com/yuque/0/2021/jpeg/anonymous/1617199282837-c09b27d5-855c-4741-bbac-71f4a775685e.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*khrYRYi6VN0AAAAAAAAAAAAADvuFAQ/original)
    
*   ![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*khrYRYi6VN0AAAAAAAAAAAAADvuFAQ/original)
    
*   ![](https://cdn.nlark.com/yuque/0/2021/png/22896906/1633760844985-avatar/8d940ff5-eb9f-4de0-8712-866f92a2ef95.png?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*khrYRYi6VN0AAAAAAAAAAAAADvuFAQ/original)
    
*   ![](https://cdn.nlark.com/yuque/0/2020/jpeg/anonymous/1589863884163-7415b504-81c9-4a79-8317-0aee7bd1a517.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://cdn.nlark.com/yuque/0/2023/jpeg/anonymous/1687270471652-05531eea-455d-4a4e-8667-e162aad82957.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    
*   ![](https://cdn.nlark.com/yuque/0/2023/jpeg/anonymous/1686823855622-61b92198-a250-4a6c-b409-ac07cdd9c953.jpeg?x-oss-process=image%2Fresize%2Cm_fill%2Cw_64%2Ch_64%2Fformat%2Cpng)
    

13

[macrozheng](/macrozheng)

2023-05-15 16:34

6696

IP 属地江苏

举报

分享到：[](https://service.weibo.com/share/share.php?url=https%3A%2F%2Fwww.yuque.com%2Fmacrozheng%2Fmall-learning%2Ftcgyq9zxgeggq80z&pic=null&title=mall%E9%A1%B9%E7%9B%AE%E6%9E%B6%E6%9E%84%E5%8F%8A%E5%8A%9F%E8%83%BD%E6%A6%82%E8%A7%88%20%7C%20%E6%9C%AC%E8%8A%82%E8%AF%BE%E7%A8%8B%E4%BD%9C%E4%B8%BA%E3%80%8Amall%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B%E3%80%8B%E7%9A%84%E5%BC%80%E7%AF%87%EF%BC%8C%E4%B8%BB%E8%A6%81%E5%AF%B9mall%E9%A1%B9%E7%9B%AE%E4%B8%AD%E4%BD%BF%E7%94%A8%E7%9A%84%E6%8A%80%E6%9C%AF%E3%80%81%E5%8A%9F%E8%83%BD%E5%8F%8A%E6%95%B0%E6%8D%AE%E5%BA%93%E8%A1%A8%E8%BF%9B%E8%A1%8C%E4%BB%8B%E7%BB%8D%EF%BC%8C%E5%B8%8C%E6%9C%9B%E5%A4%A7%E5%AE%B6%E8%83%BD%E5%AF%B9mall%E9%A1%B9%E7%9B%AE%E6%9C%89%E6%89%80%E4%BA%86%E8%A7%A3%E3%80%82mall%E9%A1%B9%E7%9B%AE%E7%AE%80%E4%BB%8Bmall%E9%A1%B9%E7%9B%AE%E6%98%AF%E4%B8%80%E5%A5%97%E7%94%B5%E5%95%86%E7%B3%BB%E7%BB%9F%EF%BC%8C%E5%8C%85%E6%8B%AC%E5%89%8D%E5%8F%B0%E5%95%86%E5%9F%8E%E7%B3%BB%E7%BB%9F%E5%8F%8A%E5%90%8E%E5%8F%B0%E7%AE%A1%E7%90%86%E7%B3%BB%E7%BB%9F%EF%BC%8C%E5%9F%BA%E4%BA%8ESpringBoot%2BMyBatis%E5%AE%9E%E7%8E%B0%E3%80%82%E5%89%8D%E5%8F%B0%E5%95%86%E5%9F%8E%E7%B3%BB%E7%BB%9F%E5%8C%85%E5%90%AB%E9%A6%96%E9%A1%B5%E9%97%A8%E6%88%B7%E3%80%81%E5%95%86%E5%93%81%E6%8E%A8%E8%8D%90%E3%80%81%E5%95%86%E5%93%81%E6%90%9C...)

划词评论（0）

![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*khrYRYi6VN0AAAAAAAAAAAAADvuFAQ/original)

返回文档

正文

14px

正文

Ctrl + ⇧ + F全屏编辑

  

回复

![](https://mdn.alipayobjects.com/huamei_0prmtq/afts/img/A*IVdnTJqUp6gAAAAAAAAAAAAADvuFAQ/original)

[关于语雀](/help/about)[使用帮助](/help)[数据安全](/about/security)[服务协议](/terms)[English](?language=en-us)

[](/dashboard)[macrozheng](/macrozheng "macrozheng")

mall学习教程

搜索Ctrl + J

首页

目录

序章

[

mall项目架构及功能概览

](/macrozheng/mall-learning/tcgyq9zxgeggq80z)

[

mall项目核心功能演示

](/macrozheng/mall-learning/sriorzcgksa20yhu)

[

mall项目学习所需知识点

](/macrozheng/mall-learning/nadzq6parofn2666)

[

mall项目学习思路及课程介绍

](/macrozheng/mall-learning/ou7todk48ltgfti8)

架构篇

[

mall项目架构篇介绍

](/macrozheng/mall-learning/hykdqpb2s8n4t7yk)

[

SpringBoot使用教程

](/macrozheng/mall-learning/akwxi9s0nvxwo5om)

[

SpringBoot常用注解

](/macrozheng/mall-learning/lg6fchmsop89bay0)

[

MyBatis使用教程

](/macrozheng/mall-learning/txnct43oglw7iin6)

[

MyBatis Generator使用教程

](/macrozheng/mall-learning/bggbgeqnrpg5ugvw)

[

Lombok使用教程

](/macrozheng/mall-learning/ms4yeraziz18rbxi)

[

Hutool使用教程

](/macrozheng/mall-learning/dmqfpr6p5n44yp4p)

大纲

[mall项目简介](#tbHe1)

[项目演示](#Ehj8V)

[后台管理系统](#nNWYB)

[移动端商城](#w7Oqu)

[mall中使用的技术](#DR0Av)

[后端技术](#U1Ar4)

[前端技术](#k5zxL)

[移动端技术](#M9nnr)

[mall实现的功能概览](#u8Q6p)

[后台管理系统](#FBmV0)

[移动端商城](#wD1WY)

[mall数据库表概览](#Wp7xS)

[数据库表前缀说明](#ujZmb)

Adblocker

Press space bar to start a drag. When dragging you can use the arrow keys to move the item around and escape to cancel. Some screen readers may require you to be in focus mode or to use your pass through key