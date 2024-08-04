# npm 遇到的那些事

## 安装卡住不动了 直接超时了 TIMEOUT

很明显是网络问题，或者 NOT FOUND PACKAGE，可以尝试使用默认的镜像源。

1. 查看配置 `npm config list`

2. 配置NPM的PROXY代理 `npm config set proxy http://`

3. 配置NPM的HTTPS-PROXY代理 `npm config set https-proxy http://`

一定要使用默认的镜像源，不然会出现很多问题。

可以在PROXY的日志中查看是否有正确的数据流动。防止TIMEOUT。