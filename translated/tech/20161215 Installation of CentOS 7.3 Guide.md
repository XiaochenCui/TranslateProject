CentOS 7.3 安装指南
============================================================

基于 Red Hat 企业版的最新版本的 CentOS 7 在今年的 11 月发布了，包含了许多 bug 修复和包更新,比如 Samba、Squid、libreoffice、SELinux、systemd 等，并支持第七代 Intel 酷睿 i3、i5、 i7 处理器。

本指南将向你展示如何在 UEFI 的机器上使用 DVD ISO 镜像来安装 CentOS 7.3。

如果你在查找 **RHEL**，看下我们的 [RHEL 7.3 安装指南][2]

#### 要求

1.  [下载 CentOS 7.3 ISO 镜像][1]

要在 UEFI 的机器上正确安装C entOS 7.3，首先按键（(`F2`、 `F11`、 `F12`，取决与你的主板类型）进入主板的 UEFI 的设置，并且确保 QuickBoot/FastBoot以及 Secure Boot 已被禁用。

### CentOS 7.3安装

1. 在你从上面的链接下载完成镜像之后，使用 [Rufus][3] 工具将它烧录到 DVD 或者创建一个可启动的 UEFI 兼容 USB 盘。

将 USB/DVD 放入主板驱动器中，重启电脑并用特定的功能键（`F12`、 `F10`，取决于主板供应商）让 BIOS/UEFI 从 DVD/USB 启动。

ISO 镜像启动完成后，你机器上会显示一个页面。在菜单中选择 **Install CentOS 7** 并按下回车继续。

[
 ![CentOS 7.3 Boot Menu](http://www.tecmint.com/wp-content/uploads/2016/12/CentOS-7.3-Boot-Menu.png) 
][4]

*CentOS 7.3 启动菜单*

2. 在安装镜像加载到内存完成后，会显示一个欢迎页面。选择你在安装中使用的语言并按下**继续**按钮。

[
 ![Select CentOS 7.3 Installation Language](http://www.tecmint.com/wp-content/uploads/2016/12/Select-CentOS-7.3-Installation-Language.png) 
][5]

*选择 CentOS 7.3 安装语言*

3. 在下一个页面点击**日期和时间**，从地图中选择你的地理位置。确认正确配置了日期和时间，并点击**完成**回到主安装界面。

[
 ![CentOS 7.3 Installation Summary ](http://www.tecmint.com/wp-content/uploads/2016/12/CentOS-7.3-Installation-Summary.png) 
][6]

*CentOS 7.3 安装总结*

[
 ![Select Date and Time](http://www.tecmint.com/wp-content/uploads/2016/12/Select-Date-and-Time.png) 
][7]

*选择日期和时间*

4. 点击**键盘**菜单进入键盘布局页面。选择或者添加一个键盘布局并点击**完成**继续。

[
 ![Select Keyboard Layout](http://www.tecmint.com/wp-content/uploads/2016/12/Select-Keyboard-Layout.png) 
][8]

*选择键盘布局*

5. 接下来，添加或者配置一个你系统中的语言并点击**完成**进入下一步。

[
 ![Select Language Support](http://www.tecmint.com/wp-content/uploads/2016/12/Select-Language-Support.png) 
][9]

*选择语言支持*

6. 在这步中，你可以通过选择列表中安全配置来设置你的系统**安全策略**。

点击**选择配置**按钮，选择你想要的安全配置，并点击**应用安全设置**按钮到 **On**。点击**完成**后继续安装。

[
 ![Enable CentOS 7.3 Security Policy](http://www.tecmint.com/wp-content/uploads/2016/12/Enable-CentOS-7-Security-Policy.png) 
][10]

*启用 CentOS 7.3 安全策略*

7. 下一步，点击**软件选择**按钮来配置基础机器环境。

从左边的列表，你可以选择安装桌面环境（**Gnome、KDE Plasma 或者创造型工作站**），或者选择一个服务器自定义安装类型（Web 服务器、计算节点、虚拟化主机、基础设施服务器、带图形界面的服务器或者文件及打印服务器），或者执行一个最小化的安装。

为了随后能自定义你的系统，选择**最小化**带兼容库安装，点击完成按钮继续。

[
 ![CentOS 7.3 Software Selection](http://www.tecmint.com/wp-content/uploads/2016/12/CentOs-7.3-Software-Selection.png) 
][11]

*CentOS 7.3 软件选择*

对于完整的 **Gnome 或者 KDE** 桌面环境，使用下面的截图作为指引。

[
 ![Gnome Desktop Software Selection](http://www.tecmint.com/wp-content/uploads/2016/12/Gnome-Desktop-Software-Selection.png) 
][12]

*Gnome 桌面软件选择*

[
 ![KDE Desktop Software Selection](http://www.tecmint.com/wp-content/uploads/2016/12/KDE-Desktop-Software-Selection.png) 
][13]

*KDE 桌面软件选择*

8. 假设你要在服务器上安装一个**图形用户界面**，从左栏选择**<ruby>带GUI的服务器<rt>Server with GUI</rt></ruby>**，并在右栏中根据服务器要提供给客户端的服务选择合适的附加软件。

你可以选择的服务是非常多样化的，从备份、DNS 或者 e-mai 服务到文件存储服务、FTP、HA 或者[监控工具][14]。只选择对你网络设置最重要的服务。

[
 ![Select Server with GUI](http://www.tecmint.com/wp-content/uploads/2016/12/Select-Server-with-Gui.png) 
][15]

*选择带 GUI 的服务器*

9. 使用默认**安装源**，以防没有使用其它特定的网络位置，比如 HTTP、HTTPS、FTP 或者NFS 协议作为额外的仓库，并点击安装位置来创建一个磁盘分区。

在设备选择页面，确保你已经选择了本地磁盘。同样，在其他存储选项中确保选择了自动配置分区。
in case you’re not using other specific network locations such as HTTP, HTTPS, FTP or NFS protocols as additional repositories and hit on Installation Destination in order to create hard disk partitions.
这个选项可以确保你的磁盘会根据磁盘空间和Linux文件系统层次结构被正确分区。它会为你自动创建/（root）、/home和swap分区。点击完成来应用磁盘分区计划并回到主安装界面。

重要提醒：如你你想要创建自定义分区及自定义分区大小，你可以选择“I will configure partitioning”选项来创建自定义分区。

[
 ![Select CentOS 7.3 Installation Destination](http://www.tecmint.com/wp-content/uploads/2016/12/Select-CentOS-7.3-Installation-Destination.png) 
][16]

安装CentOS 7.3安装位置

10. 接下来，如果你想要释放系统内存，点击KDUMP选项并禁用它。点击完成并回到主安装界面。

[
 ![Kdump Selection](http://www.tecmint.com/wp-content/uploads/2016/12/Kdump-Selection.png) 
][17]

Kdump选择

11. 在下一步中设置你的主机名并启用网络服务。点击网络和主机名，在主机名中输入你的FQDN（完整网域名称），万一你在局域网中有一个DHCP服务器将以太网按钮从OFF切换到ON来激活网络接口。

[
 ![Set Network and Hostname](http://www.tecmint.com/wp-content/uploads/2016/12/Set-Network-Hostname.png) 
][18]

设置网络及主机名

12. 为了静态配置你的网络接口，点击配置按钮，手动如截图所示添加IP设置，并点击保存按钮来应用更改。完成后，点击完成按钮来回到主安装菜单。

[
 ![Configure Network and IP Address](http://www.tecmint.com/wp-content/uploads/2016/12/Configure-Network-and-IP-Address.png) 
][19]

配置网络和IP地址

13. 最后检查下所有到目前为止的配置，如果一切没问题，点击开始安装按钮开始安装。

[
 ![Begin CentOS 7.3 Installation Guide](http://www.tecmint.com/wp-content/uploads/2016/12/Begin-CentOS-7.3-Installation.png) 
][20]

开始CentOS 7.3安装向导

14. 开始安装后，一个新的设置用户界面会显示出来。首先点击root密码并添加一个强密码。

root账户是每个Linux系统的最高管理账户密码，它拥有所有的权限。设置完成后点击完成按回到用户设置界面。

[
 ![Select Root Password](http://www.tecmint.com/wp-content/uploads/2016/12/Select-Root-Password.png) 
][21]

选择root密码

[
 ![Set Root Password](http://www.tecmint.com/wp-content/uploads/2016/12/Set-Root-Password.png) 
][22]

设置root密码

15 用root账户运行系统是非常不安全和危险的，因此建议你点击创建用户按钮创建一个新的系统账户来[执行每日的系统任务][23]、

添加新的用户，并同时选择下面的两个选项来授予用户root权限以及每次在登录系统时手动输入密码。

当你完成最后一项点击完成按钮并等待安装完成。

[
 ![Create User Account](http://www.tecmint.com/wp-content/uploads/2016/12/Create-User-Account.png) 
][24]

创建用户账户

16. 几分钟后安装程序会报告CentOS已经成功安装在你机器中。要使用系统，你只需要移除安装媒介并重启机器。

[
 ![CentOS 7.3 Installation Complete](http://www.tecmint.com/wp-content/uploads/2016/12/CentO-7.3-Installation-Complete.png) 
][25]

CentOS 7.3安装完成

17. 重启之后，使用安装中创建的用户登录系统，并且用root权限执行下面的命令来执行系统更新。

```
$ sudo yum update
```
[
 ![Update CentOS 7.3](http://www.tecmint.com/wp-content/uploads/2016/12/Update-CentOS-7.3.png) 
][26]

更新CentOS 7.3

所有[yum管理器][27]的问题都选择`yes`，最后再次重启电脑（使用sudo init 6）来应用新的内核升级。

```
$ sudo init 6
```

就是这样！在你的机器中享受最新的CentOS 7.3吧。


------------------

作者简介:

Matei Cezar

![](http://2.gravatar.com/avatar/be16e54026c7429d28490cce41b1e157?s=128&d=blank&r=g)

我是一个电脑上瘾的家伙，一个开源和linux系统软件的粉丝，有大约4年的Linux桌面，服务器和bash脚本的经验。

--------------------------------------------------------------------------------

via: http://www.tecmint.com/centos-7-3-installation-guide/

作者：[Matei Cezar][a]
译者：[geekpi](https://github.com/geekpi)
校对：[jasminepeng](https://github.com/jasminepeng)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]:http://www.tecmint.com/author/cezarmatei/
[1]:http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-DVD-1611.iso
[2]:http://www.tecmint.com/red-hat-enterprise-linux-7-3-installation-guide/
[3]:https://rufus.akeo.ie/
[4]:http://www.tecmint.com/wp-content/uploads/2016/12/CentOS-7.3-Boot-Menu.png
[5]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-CentOS-7.3-Installation-Language.png
[6]:http://www.tecmint.com/wp-content/uploads/2016/12/CentOS-7.3-Installation-Summary.png
[7]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-Date-and-Time.png
[8]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-Keyboard-Layout.png
[9]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-Language-Support.png
[10]:http://www.tecmint.com/wp-content/uploads/2016/12/Enable-CentOS-7-Security-Policy.png
[11]:http://www.tecmint.com/wp-content/uploads/2016/12/CentOs-7.3-Software-Selection.png
[12]:http://www.tecmint.com/wp-content/uploads/2016/12/Gnome-Desktop-Software-Selection.png
[13]:http://www.tecmint.com/wp-content/uploads/2016/12/KDE-Desktop-Software-Selection.png
[14]:http://www.tecmint.com/command-line-tools-to-monitor-linux-performance/
[15]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-Server-with-Gui.png
[16]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-CentOS-7.3-Installation-Destination.png
[17]:http://www.tecmint.com/wp-content/uploads/2016/12/Kdump-Selection.png
[18]:http://www.tecmint.com/wp-content/uploads/2016/12/Set-Network-Hostname.png
[19]:http://www.tecmint.com/wp-content/uploads/2016/12/Configure-Network-and-IP-Address.png
[20]:http://www.tecmint.com/wp-content/uploads/2016/12/Begin-CentOS-7.3-Installation.png
[21]:http://www.tecmint.com/wp-content/uploads/2016/12/Select-Root-Password.png
[22]:http://www.tecmint.com/wp-content/uploads/2016/12/Set-Root-Password.png
[23]:http://www.tecmint.com/file-and-directory-management-in-linux/
[24]:http://www.tecmint.com/wp-content/uploads/2016/12/Create-User-Account.png
[25]:http://www.tecmint.com/wp-content/uploads/2016/12/CentO-7.3-Installation-Complete.png
[26]:http://www.tecmint.com/wp-content/uploads/2016/12/Update-CentOS-7.3.png
[27]:http://www.tecmint.com/20-linux-yum-yellowdog-updater-modified-commands-for-package-mangement/