# NCST-Fourth-semester-of-college

大学第四学期

git config --global http.sslVerify "false"  关闭了ssl让某个东西不在安全

## 一、禁用

1.使用git向GitHub传项目时报错：`fatal: unable to access "xxx": OpenSSL SSL_read:Connection was reset, errno 10054`
禁用证书命令：`git config --global http.sslVerify "false"`
借鉴：[https://blog.csdn.net/a157796...](https://link.segmentfault.com/?enc=lrvUAnlis25SDkl2hlHo7w%3D%3D.XWUWmZAlaFBneqEV4XHSd%2FIRNvhvGR052t14AfxgxjtlvmpXoqJPYTwWwAPb79Pc2AemDKTOd4QDTM5z1lUnMg%3D%3D)

2.当你通过HTTPS访问Git远程仓库，如果服务器的SSL证书未经过第三方机构签署，那么Git就会报错。这是十分合理的设计，毕竟未知的没有签署过的证书意味着很大安全风险。但是，如果你正好在架设Git服务器，而正式的SSL证书没有签发下来，你为了赶时间生成了自签署的临时证书，怎样才是最便捷的测试手段。

禁用证书命令：（--global是全局的意思）
`git config http.sslVerify"false"`
或 `git config --global http.sslVerify false`
或 `git config --global http.sslVerify "false"`
借鉴：[https://www.jianshu.com/p/df4...](https://link.segmentfault.com/?enc=%2FEsn7AtuggzP5%2FhBOxb1qQ%3D%3D.FDyofB68QAPE%2Bvtn%2BVwRzMn40zQZwQDKnQbGNk0LVRgyl23x4rQY8bvXBOJf4WeL)

## 二、启用

使用 `$ git push -u origin main`后弹出警告：`TLS certificate verification has been disabled!`
**重新启用证书命令：**
`git config --global http.sslVerify true`
（这个为什么加粗呢，因为有的博客只说了忽略，没说怎么重新启用证书）

没办法在手机版Github上新增文件 但是可以写

git可以追踪一行行的，不能追踪二进制文件




大二最后几节课了，期末复习真烦人了

感觉自己的成长不快不慢吧

就这样了

江湖相逢，再相忘与互联网
