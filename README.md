### 本项目为weixin-java-tools的Demo演示程序，基于Spring Boot构建，实现微信企业号后端开发功能。
更多信息请查阅：https://github.com/Wechat-Group/weixin-java-tools

[![Build Status](https://travis-ci.org/binarywang/weixin-java-cp-demo.svg?branch=master)](https://travis-ci.org/binarywang/weixin-java-cp-demo)
-----------------------

## 使用步骤：
1. 配置：复制 `/src/main/resources/application.yml.template` 或者修改其扩展名生成 `application.yml` 文件，根据自己需要填写相关配置（需要注意的是：yml文件内的属性冒号后面的文字之前需要加空格，可参考已有配置，否则属性会设置不成功）；	
1. 运行Java程序：`WxCpDemoApplication`；
1. 打开shell或cmd，进入ngrok目录，运行 `ngrok -config ngrok.cfg -subdomain my-domain 8080` 如果运行失败，请更换my-domain为其它字符串，直至连接成功；
1. 配置微信企业微信对应应用中的“接受消息”部分的“接收消息服务器配置”URL地址：http://my-domain.tunnel.qydev.com/wx/cp/portal （注意my-domain要跟上面的一致，需要符合微信官方的要求）；
1. 根据自己需要修改各个handler的实现，加入自己的业务逻辑。
	
