### 安装 cpolar

> cpolar 是一款内外穿透软件，非常方便且免费

官网下载软件：https://www.cpolar.com

注册用户，选择免费版本

直接安装即可

<br>

打开 `cpolar gui.exe`

此时打开的网页选择创建隧道，按照下图方式对 3306 端口进行内网穿透

![](../img/sql/cpolar/cq1.png)

<br>

点击一次创建后即可选择“隧道列表”，找到我们刚刚创建的隧道，点击启动；

于“在线隧道列表”内查看当前隧道状态，记下公网地址！

![](../img/sql/cpolar/cq2.png)

<br>

### 链接 mysql

> 省略 mysql 的安装过程！

打开 navcat，新建一个链接

按照以下格式填写：

1. 主机名：随便取
2. 主机：去掉开头的 `tcp://` 以及结尾的端口号后剩下的内容
3. 端口：填写公网地址的端口！不是 3306！！！
4. 账户密码：你安装 mysql 设置的直接写进去就好了

![](../img/sql/cpolar/cq3.png)

<br>

直接点击链接就可以连接到我们的数据库了

该方法亦可以在虚拟机而非物理机上实现！

<br>
