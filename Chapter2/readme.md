# 用户模式实现的功能

```shell
strace
sar -P ALL 1
```


## loop

```shell
./loop &
# 查看进程号
ps aux | grep ./loop | grep -v grep | awk '{print $2}'
# 查看进程的状态
sar -P ALL 1
```
问题: 为什么书上写的占用是 %user 但我是 %nice, 我使用 WSL-Debian 和 LXC-Debian 都是这样的
