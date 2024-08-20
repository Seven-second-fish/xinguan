# xinguan
新冠-物资管理系统，毕业设计程序

模块划分
xinguan-business: 业务模块,所有与业务相关的代码放在此工程中。
xinguan-system: 系统模块,权限控制相关的代码放在此工程中。
xinguan-common: 公共模块,存放工具类、领域模型（DTO）、数据模型对象(DO)一些通用的类。
xinguan-generator: 代码生成器，生成Controller,Service,ServiceImpl,以及前端代码。
xinguan-vue: 前端项目, npm install 安装依赖后, npm run serve 启动该项目。
xinguan-web: 处理前端请求的Controller,放在此工程中。

技术栈
SpringBoot, Shiro ,Swagger-UI,mybatis,JWT,Mysql,Vue.js+element-ui

启动步骤
1.在vue前端xinguan-vue项目根目录下运行cmd命令，输入cnpm install按照vue项目依赖（前提是有nodejs环境，最好用cnpm安装下）等待安装成功。
2.新建数据库xinguan,导入数据库文件xinguan.sql
3.导入Xinguan后端项目进入idea或eclipse开发环境中，配置Xinguan\xinguan-web\src\main\resources\application-dev.yml文件修改连接串5-7行，改为本机数据库地址和账户密码
4.运行Xinguan\xinguan-web\src\main\java\com\coderman\XinguanApplication.java文件（右击run as application），完成后台的启动
5.在vue前端项目根目录下运行cmd命令，输入命令npm run dev  启动前端项目
6.浏览器访问项目地址即可进入系统，用户名和密码为  admin/123456
