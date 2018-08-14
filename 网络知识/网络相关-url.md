### url

- uri

- url


URL只能使用英文字母、阿拉伯数字和某些标点符号，不能使用其他文字和符号。这是因为
网络标准[RFC 1738](http://www.ietf.org/rfc/rfc1738.txt)做了硬性规定

一个url（统一资源定位符）的主要结构：
https://www.google.com/search?q=sdfs&oq=sdfs&aqs=chrome

scheme:http or https
host:www.google.com
path:search
params:q=sdfs&oq=sdfs&aqs=chrome

----

一、概念
URL：统一资源定位符 (Uniform Resource Locator, URL)。

完整的URL由这几个部分构成：scheme://host:port/path?query#hash：

scheme：通信协议，常用的有http、https、ftp、mailto等。
host：主机域名或IP地址。
port：端口号，可选。省略时使用协议的默认端口，如http默认端口为80。
path：路径由零或多个"/"符号隔开的字符串组成，一般用来表示主机上的一个目录或文件地址。
query：查询，可选。用于传递参数，可有多个参数，用"&"符号隔开，每个参数的名和值用"="符号隔开。
hash：信息片断字符串，也称为锚点。用于指定网络资源中的片断。

二、举例

比如URL如下，https://www.baidu.com/index.html?id=1&page=1#name1

用javascript获得其中的各个部分如下：
window.location.href：整个URl字符串，返回值："https://www.baidu.com/index.html?id=1&page=1#name1"。
window.location.protocol：协议部分，返回值："https:"。
window.location.host：主机部分。返回值："www.baidu.com"。
window.location.port：端口部分。如果采用了协议默认的端口，则返回空字符。本例返回值：""。
window.location.pathname：路径部分。返回值："/index.html"。
window.location.search：查询(参数)部分。返回值："?id=1&page=1"。
window.location.hash：锚点。返回值："#name1"。

----

The components of the URL are combined and delimited as follows:
scheme://host:port/path?querycopy to clipboard
The scheme is followed by a colon and two forward slashes.
If a port number is specified, that number follows the host name, separated by a colon.
The path name begins with a single forward slash.
If a query string is specified, it is preceded by a question mark.
Figure 1. Syntax of an HTTP URL
Read syntax diagramSkip visual syntax diagram
                            .-:80-----.                      
>>-http://--+-host name--+--+---------+--/--path component------>
            '-IP address-'  '-:--port-'                      

>--+-----------------+-----------------------------------------><
   '-?--query string-'   

---

[菜鸟教程](http://www.runoob.com/html/html-url.html)

http://www.cnblogs.com/01picker/p/4434197.html

[http详细文档](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Overview)

[url结构](https://www.bh-lay.com/blog/14b531db64a)

[计算机网络基础知识总结](http://www.cnblogs.com/maybe2030/p/4781555.html)

[阮一峰：网络基础知识](http://www.ruanyifeng.com/blog/2010/02/url_encoding.html)