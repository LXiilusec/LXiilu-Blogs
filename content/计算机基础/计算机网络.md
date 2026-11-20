[HTTP](#HTTP)
[TCP](#TCP)
[http报文格式](#http报文格式)
[头部字段](#头部字段)
[缓存规则](#缓存规则)
[连接规则](#连接规则)

# IP 域名 端口

* IP: 是网络中每一台设备的唯一标识，能精准定位设备的GPS地址。
* 域名：？？
* 端口：用于区分不同的服务
* IP和域名的关系：一个IP可以有多个域名，一个域名只有一个IP；（不理解）
* 
![[Pasted image 20261105001538.png]]

# http  https
## http:

* HTTP ( 全称为 " 超文本传输协议",英文Hyper Text Transfer Protocol ) 是一种应用非常广泛的 应用层协议.
超文本的解释:所谓超文本指的是传输的内容不止是文本内容(html,css),还可能是一些其它资源,如音频,图片,视频等。
* 我的理解：是一个查询数据的工具，我发出请求，通过这个协议分析确定我要找的东西，在响应返还给我。

## https 
* emmm... 可以理解是http的plus版本？给它要传输的数据进行了加密，防止在传输过程中被窃取。
* 常见的加密方式：1.对称加密，2.非对称加密，3.哈希函数（看不懂）。







# TCP
* 传输控制协议
*  **建立连接**
   “三次握手”
   客户端：发送连接请求
   服务器：确认请求并回应
   客户端：确认回应
* 传输数据
* **断开连接**
  “四次挥手”
   客户端:发送断开请求
   服务器：确认收到
   服务器：发送断开请求
   客户端：确认收到请求

# HTTP
* 应用层协议
* ![[Pasted image 20261106142423.png|528]]

# http报文格式
## 请求报文
![[Pasted image 20261106143925.png]]
* 常见方法：GET（获取资源）、POST（提交数据）、PUT（上传文件）等。
* ![[Pasted image 20261106185653.png]]
* cookie:![[Pasted image 20261106190227.png]]
## 响应报文
* 首行
* ![[Pasted image 20261106194355.png]]
* 关键状态码：
  200：成功
  404：资源未找到
  500：服务器内部错误

## URL
* 格式：协议://域名:端口/路径？查询参数#片段
   例 ：https://www.example.com:443/search?q=HTTP#results

## 头部字段

![[Pasted image 20261106200437.png]]
* 例子
![[Pasted image 20261106200605.png]]
* host: 要访问的网站
* User-Agent: 说明我的浏览器，操作系统，设备。
* Referer:表示是从哪个页面过来的。
* Accept: 内容协商。同一个 URL，浏览器要 HTML，API 客户端要 JSON，服务器按 Accept 返回不同格式。
  ![[Pasted image 20261106201739.png]]
* Accept-Language: 返回对应语言版本的页面,优先中文，其次英文。
* Accept-Encoding:服务器把响应压缩,加载更快。
* Authrization: 正式的“认证凭据”，常用于 API 调用。
* 
### 缓存规则
* Cache-Control：存储规则。
 * ![[Pasted image 20261106202803.png]]
 * If-Modified-Since：
 * ![[Pasted image 20261106203025.png]]
（不太理解）

### 连接规则
* connection：
![[Pasted image 20261106203422.png]]*
* upgrade : 
  ![[Pasted image 20261106203710.png]]
  (没看懂)


