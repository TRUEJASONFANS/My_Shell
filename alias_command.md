## 杀死所有符合“命名” 的进程
```
ps -u zhxie | grep python | awk '{print $1}' | xargs kill -9
```