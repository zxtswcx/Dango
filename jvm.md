````
# 11656 进程id
# 10000 毫秒，每10000毫秒输出一次
# 30 输出30次
jstat -gc -t 11656 10000 30
# 11656 进程id
jstack 11656
# 查看进程下哪些线程占用了高的cpu
top -p 11656 -H

jmap -dump:format=b,file=/tmp/xxx.dat 1039
jhat -port 8039 xxx.dat

## 参数
-XX:+HeapDumpOnOutOfMemoryError
````

