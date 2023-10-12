# 【Linux】Linux常用指令清单

{% hint style="info" %}
**不会用Linux的程序员不是好的程序员。**
{% endhint %}

## 分布式训练

1. mp.spawn()需要写明\_ \__main_ \_\_函数，不然会递归创造子进程

比如下图，一开始读取data没有放进\_ \__main_ \_\_导致读了三遍数据。。。。。。

2. 码一个PyTorch介绍多GPU训练的官方教程（印度人我的神！！！！！！！）

https://github.com/pytorch/examples/tree/main/distributed/ddp-tutorial-series

## linux查看文件夹占用空间和磁盘使用量和显存

1.查看当前目录下**各文件夹**占用了多少空间

du -sh ./\*

使用时可以加上sudo使用

![image-20230321170332981](https://c/Users/AinsleyWilde233/AppData/Roaming/Typora/typora-user-images/image-20230321170332981.png)

2.查看每个**磁盘**用了多少空间，还剩多少空间，以及挂载的目录位置

```
df -h 
df -lh
// 不是sudo也可以
```

3.查看**显卡**使用情况

查看某一块GPU

```
nvidia-smi -i n #n是GPU编号
```

查看所有GPU

```
fuser -v /dev/nvidia*
```

查看文件详细属性（修改时间）

```
ls -l
```



![image-20230321202631134](C:%5CUsers%5CAinsleyWilde233%5CAppData%5CRoaming%5CTypora%5Ctypora-user-images%5Cimage-20230321202631134.png)

## python import 路径问题

```
os.chdir("../../photo")
sys.path.append
```

```python
# python程序的相对路径是基于main函数所在单位文件来的
# 同级 ./
# 上一级 ../
# windows需要使用转义符\，但似乎写相对路径的时候用哪个都可以
```

## tmux多会话

新建

```linux
tmux new -s session_name
```

分离会话

```
tmux detach
```

接入会话

```
tmux attach -t id/sessionname
```

结束对话

```
tmux kill-session -t id/name
```

切换对话

```
tmux switch -t id/name
```

重命名

```
tmux rename-session -t old_id/old_name new_name
```

显示当前所有对话

```
tmux ls
```

## Loss

{% embed url="https://www.cnblogs.com/nekoneko-15/p/13691338.html" %}



&#x20;:thumbsup:_——Powered By N.KO 唐_
