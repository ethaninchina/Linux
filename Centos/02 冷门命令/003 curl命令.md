### 使用命令curl获取http状态码
- 获取域名baidu.com（对于http、https、重定向均适用）返回的状态码
```
# curl -I -L -s --connect-timeout 5 -m 5 -o /dev/null -w %{http_code} baidu.com
```

- curl相关参数
```
-I, --head                     Show document info only
-L, --location                 Follow redirects (H) 
-s, --silent                   Silent mode. Don't output anything
--connect-timeout SECONDS      Maximum time allowed for connection
-m, --max-time SECONDS         Maximum time allowed for the transfer
-o, --output FILE              Write output to <file> instead of stdout
-w, --write-out FORMAT         What to output after completion
```
