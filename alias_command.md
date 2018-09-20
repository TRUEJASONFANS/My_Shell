## 杀死所有符合“命名” 的进程
```
ps -u zhxie | grep python | awk '{print $1}' | xargs kill -9
```
## 找到目录夹下所有 jar 并移动到指定位置
```
find ./ -name "*.pl"|awk '{printf("mv %s dir\n", $ARGV[0])}' | sh 
```
## 查看某端口占用的程序 
lsof -i：port 
