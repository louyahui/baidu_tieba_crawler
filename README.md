# baidu_tieba_crawler
##[演示地址](http://www.femirror.com/index)
服务器很慢，请原谅
### 一定要安装redis以及开启redis服务！！！
##1.3更新说明
* 使用redis队列爬取 所有爬取任务都会插入到队列 实现后台爬取
* socket 只用于通讯，其他接口均换成http请求
* 增加了右边的队列的监控

##更迭期望
* 数据分析 
* 任务队列，实现无需驻足网页爬取，而是后台爬取
* 代码优化 部分重写

##项目地址
https://github.com/tyaqing/baidu_tieba_crawler
喜欢的给个star
#使用说明书
！！！爬虫类的东东还是友善使用
### 程序运行不起来就要检查下 以下接口是否替换
~ 代理的api接口  mongo地址 socket地址 ~

##真·调试
```
npm i          //安装后端依赖
node server.js //运行restful api 和socket服务 默认端口8081
cd fe          //进入前端目录
npm i          //安装前端依赖
npm run dev    //运行调试模式  默认端口8080
```
*@Molunerfinn 谢谢建议*
##关于技术栈
用到的东西挺多的，但是都是用了点皮毛知识,提前踩坑。
####前端的
vue大礼包(vue-resource vue-router vue-socket.id element-ui)
####后端的
express socket.io superagent cheerio mongoose kue
####数据库
mongo
