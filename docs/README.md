# 目录

## 项目介绍

学之思在线考试系统是一款 java + vue 的前后端分离的考试系统。主要优点是开发、部署简单快捷、界面设计友好、代码结构清晰。目前支持web端和微信小程序，能覆盖到pc机和手机等设备。

## 开源版使用须知

仅用个人学习

禁止将本项目的代码和资源进行任何形式的出售，产生的一切任何后果责任由侵权者自负

## 演示地址

官网：<http://www.mindskip.net>

学之思考试系统：<http://www.mindskip.net/xzs.html>

学多多考试系统：<http://www.mindskip.net/xdd.html>

思多多智能考试平台：<http://www.mindskip.net/sdd.html>

## 学之思仓库版本地址

gitee - postgresql ：[https://gitee.com/mindskip/uexam](https://gitee.com/mindskip/uexam)

gitee - mysql ：[https://gitee.com/mindskip/xzs-mysql](https://gitee.com/mindskip/xzs-mysql)

github - postgresql ：[https://github.com/mindskip/xzs](https://github.com/mindskip/xzs)

github - mysql ：[https://github.com/mindskip/xzs-mysql](https://github.com/mindskip/xzs-mysql)

## 运行环境

|  环境   | 版本  |
|  ----  | ----  |
| 操作系统  | Windows / Linux |
| Jdk  | 8 |
| Redis  | 3.0 |
| PostgreSql / Mysql  | 12.0 / 8.0 |

## 技术栈列表

### 后台系统

* spring-boot  2.1.6.RELEASE
* spring-boot-security 用户登录验证
* undertow  web容器
* postgresql/mysql 优秀的开源数据库
* redis 缓存，提升系统性能
* mybatis 数据库中间件
* hikari 速度最快的数据库连接池
* 七牛云存储

### 前台系统

* Vue.js  采用新版，使用了vue-cli3搭建的系统，减少大量配置文件
* element-ui  最流行的vue组件，采用的最新版
* vue-element-admin 最新版，对该系统做了大量精简，只保留了部分样式和控件
* echarts 图表统计
* ueditor 填空题扩展插件

## 使用教程

* redis 安装
* 进群获取到数据库脚本，创建表初始化数据，数据库名称为xzs
* 安装mysql / postgresql ，导入sql脚本

## 后端启动

* /uexam/source/xzs为后台代码，建议使用IntelliJ IDEA打开
* 打开application-dev.yml文件中，配置好postgesql/mysql、redis的服务地址
* 启动后台程序,默认端口为8000。
* 学生系统地址：<http://localhost:8000/student>
* 管理端地址：<http://localhost:8000/admin>

## 前端启动

* 前端使用webstorm或者vscode，分别打开文件夹打开源代码\source\vue\xzs-student和source\vue\xzs-admin
* 执行下面2个命令，安装node_module：

 ```npm
npm config set sass_binary_site https://npm.taobao.org/mirrors/node-sass/
npm install --registry https://registry.npm.taobao.org  
 ```

* 执行下面命令，启动前端代码

 ```npm
npm run serve
 ```

## 微信小程序启动

* 先下载好微信小程序开发工具
* 打开工具，导入代码 \source\wx\xzs-student
