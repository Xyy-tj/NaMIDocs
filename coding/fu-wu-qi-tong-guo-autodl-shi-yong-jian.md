# 【服务器】通过AutoDL使用（荐）

为了缓解实验室日益增长_的DeepLearning显卡需要和不平衡_不充分的显卡资源之间的矛盾，同时减少对宿主机环境的污染，实验室的4090服务器部署了AutoDL的私有云服务架构。



1. 注册AutoDL账号，获取个人账户ID（建议同时修改个人昵称为身份标识，便于后台管理）

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

2. 将个人ID发送给服务器管理员（目前为：ZyFan），添加至授权清单。
3. 点击“私有云”，进入私有云主机界面。

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

4. “容器实例”-“创建实例”

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

6. 创建实例界面，需选择“数据盘路径”和“镜像”选项。

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

7.  创建完成后，如需使用服务器，可点击开机，默认分配一张GPU资源（无卡模式下不分配GPU）

    <figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
8. 开机后通过Jupyter-Lab进入实例操作界面。

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
