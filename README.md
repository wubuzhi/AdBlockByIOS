# 使用手册

### 简介

本项目最早是 Fork [scomper/surge.conf](https://gist.github.com/scomper/915b04a974f9e11952babfd0bbb241a8) 定制修改而来。

---

### Function
- [x] 自动代理 / 全局代理
- [x] 解决本地 DNS 可能带来的干扰
- [x] 解决部分网站跳转问题
- [x] 可突破部分内网限制（公司、学校）
- [x] 拦截部分挖矿 JS 插件
- [x] 拦截常用应用程序及网页的行为分析
- [x] 拦截常用应用程序及网页的数据统计
- [x] 拦截常用应用程序及网页的隐私跟踪
- [x] 拦截各大购物网站的运营商劫持
- [x] 拦截 Content Security Policy 劫持
- [x] 拦截 CNNIC 根证书劫持
- [x] 屏蔽部分应用程序的启动广告
- [x] 屏蔽部分运营商劫持网页弹出的流量统计
- [x] 屏蔽部分运营商劫持网页弹出的漂浮球广告
- [x] 屏蔽常用视频广告
- [x] 屏蔽常用网站广告、其他流媒体网站广告
- [x] 屏蔽法轮功等反华势力网站
- [x] 所有国内网站直线连接
- [x] Apple 服务加速（App Store、Apple Music、Apple流媒体、iCloud备份、iCloud Drive、iTunes 等）
- [x] 国外常用网站加速（Google/Youtube/Twitter/Facebook/instagram/wikipedia/Github 等）

---

### Shadowrocket (Remote Files)

````
https://raw.githubusercontent.com/lhie1/Rules/master/Shadowrocket/Complete.conf
````

---

### MitM

简介：MitM（即 Man-in-the-middle attack，用于解密 HTTPS 的流量）

iOS：
````
iOS 9 以上的系统都需要在安装证书后到关于本机里信任证书才可使其证书有效。

1. 安装：
* Surge：配置 - 编辑配置 - HTTPS 解密 - 安装证书
* Shadowrocket：配置 - 选中Shadowrocket.conf编辑配置 - HTTPS解密 - 开启HTTPS解密 - 安装证书
* Quantumult：Settings - HTTPS - HTTPS Decryption

2. 信任：
设置 - 通用 - 关于本机 - 证书信任设置 - 信任

备注：只需要安装并信任一次，使用 JSBox 升级规则丝毫不会影响证书。
备注：不要自己去生成新证书，会导致规则与证书不匹配导致 MitM 失效直接导致无法加载的问题，导出规则后直接安装并信任就可以了。如果不小心点到了，重新运行 JSBox 导出规则即可正确安装。
````

---

### 鸣谢
* @Eval](https://twitter.com/OAuth4)
* @Scomper](https://medium.com/@scomper)
* @Neurogram](http://www.taguage.com/user?id=181456)
* @suisr9255
* @Hackl0us
* @unknownTokyo
* @Jacky Y
* @Fndroid

---

### License
* 可以拷贝、转发，但是必须提供原作者信息，同时也不能将本项目用于商业用途。
