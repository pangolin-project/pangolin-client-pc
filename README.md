## pangolin-server https代理客户端
  目前支持windows/mac os 两个 平台
## 此项目是什么？
   此客户端项目主要配合服务器https://github.com/pangolin-project/pangolin-server 来做https的代理。能够通过此代理技术来保证访问的安全性和访问很多被屏蔽的网站。
## 如何使用?
- UI 如下:
![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/gui.png)
1. 在第一个输入框输入代理服务器的连接URL字符串(此连接字符串在部署服务器端的时候会生成。例如：hs://YWRtaW46MTU0MzI3MTQxNA==@yourdomain.com:443/?caddy=1&adp=11414)
2. 点击右侧的旋转箭头按钮![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/ready-connect.png)，如果上面的打√![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/connected-2.png)的变为黄色，说明此服务器可以连接通
3. 打开浏览器，输入google.com看是否能够访问，如果能够访问则说明代理成功啦

## 如何断开:
1. 再次点击按钮![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/ready-connect.png),然后状态栏上的图标![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/disconnected-2.png)变为黄色即可

## 如何分享自己的代理链接
1. 第一种是直接将自己的连接URL发送给对方，对方下载客户端程序运行，粘贴到客户端，点击连接按钮![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/ready-connect.png)即可
2. 第二种是点击分享按钮，然后点击右边的剪刀![](https://github.com/pangolin-project/pangolin-client-pc/blob/master/html/images/copy.png)按钮，将复制好的链接地址发送给对方，对方讲此链接地址输入到浏览器粘贴即可下载客户端程序。客户端程序下载完毕后就可以将此链接URL粘贴到客户端程序，点击连接，即可进行代理了。

## 如何保存连接URL？
1. 当将连接URL粘贴到连接URL输入框后，点击最右侧的保存按钮即可。这样每次启动客户端的时候，直接点击连接即可。

## 服务器如何部署？
1. 见：https://github.com/pangolin-project/pangolin-server 的说明即可。

## 常见问题:
1. 如果客户端卡死,强杀后，浏览器无法上网 ？
  - 解决办法:重新启动客户端，然后点击退出，退出后就可以正常上网了。
2. 代理后，会不会导致访问国内的网站变慢?
  - 不会的。程序默认只代理无法访问的网址。对于可以访问的网址。不会做代理。因此不会影响不走代理的网站访问速度。
3. 客户端一切设置正常，但是还是无法访问网页，怎么办？
  - 考虑是否之前有使用类似chrome的代理插件，如果有。请先到设置——》高级-》系统 里面的代理设置。把代理插件停止。
  
## 我们的优势:
1. 由于客户端和服务器端之间采用的是tls的方式，因此，对于每一个连接的数据加密密钥都是不一样的。相比shadowsocks的协议而言，更为安全！
2. 傻瓜化的使用界面，让用户使用起来更方便，再配合服务器端的一键配置脚本。让您无需任何部署经验，仍然可以快速部署属于您自己的服务器。
3. 分享更为简单。客户端提供了一键分享的功能，让分享起来更为方便。更符合国人的习惯。

## 如何做二次开发？
1. 首先请安装nodejs的开发环境
2. git clone https://github.com/pangolin-project/pangolin-client-pc.git
3. 进入到代码根目录pangolin-client-pc
4. npm install
5. npm run dbg 项目就可以运行起来啦！
