1. 访问http://github.global.ssl.fastly.net.ipaddress.com/#ipinfo查看github的ip;
2. 编辑C:\Windows\System32\drivers\etc\hosts 文件。如下
```
151.101.44.249 github.global.ssl.fastly.net
```
3. 刷新本机DNS缓存
```
在cmd窗口输入 ipconfig /flushdns
```
