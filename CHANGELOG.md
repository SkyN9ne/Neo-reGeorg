# Change Log

### v2.0.0
    实现单 Session 多 TCP 会话，解决部分环境仅支持单 Session HTTP 通讯导致的无法使用
    支持同服务器多 URL 的请求路径，避免单路径访问频率过高
    支持自定义服务端的 HTTP 响应码
    修改了部分指令为 GET , 更接近正常请求
    去除空行与去除部分特征
    支持服务端的 DNS 解析，并默认使用 (使用本地 DNS 解析用 `--local-dns`)
    优化了错误信息输出
    修改了目录名称 scripts/ => templates/ 和 neoreg_server/ => neoreg_servers/
    移除 socks4 的支持
	移除 javascript tunnel 支持

### v1.5.0
    修复 php >= 7.1 版本，无法正常使用的问题
    修复 php 环境高占用 CPU 的问题  (特别感谢 @junmoxiao 提供的支持)
    tunnel.nosocket.php 替换 tunnel.php

### v1.4.0
    jsp(x) 不依赖内置 `base64` 方法，兼容 jdk9 及以上版本
    jsp(x) 移除 `trimDirectiveWhitespaces="true"` 兼容小于 jdk8 版本
    tunnel.tomcat.5.jsp(x) 已移除

### v1.3.0
    修复 `--cookie  JSESSIONID` 冲突，负载均衡环境，服务端找不到 session 无法使用问题

### v1.2.0
    新增 `-k debug_all (or debug_base64|debug_headers_key|debug_headers_values)` 时，关闭随机混淆，方便调试

### v1.1.0
    新增 jspx 的支持