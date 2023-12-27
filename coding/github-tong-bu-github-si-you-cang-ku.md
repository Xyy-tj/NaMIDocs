# 【Github】同步Github私有仓库

Linux系统下生成RSA格式的密钥对，一路回车即可：

```sh
ssh-keygen -t rsa
```

打开Linux的.ssh文件夹，获取公钥

```sh
cd /root/.ssh/
vi id_rsa.pub
```

复制公钥内容，下面是一个例子（以ssh-rsa开头）：

```
ssh-rsa AAAAB3NzaC1yc2E……(不予显示)……lsUltsIji60PfEf2bhexgRayWbdNJZlaXn+lXrU= root@autodl-container-879242bf41-c7ebbb9a
```

打开Github，点击右上角头像-Setting，进入SSH and GPG keys：

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

点击Net SSH Key，录入复制好的SSH公钥内容：

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

使用命令测试连接情况：

ssh -T git@github.com

```sh
ssh -T git@github.com
```

连接成功的情况下，显示：

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

然后打开私有仓库页面，复制SSH链接：

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

回到Linux终端，执行下列命令：

```sh
git clone git@github.com:Xyy-tj/Self-Evolution-Learning.git
```

完成！
