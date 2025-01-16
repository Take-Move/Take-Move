# 清华镜像源更换指南

## 备份原来的 `sources.list`
```bash
sudo mv /etc/apt/sources.list /etc/apt/sources.list.bak
sudo gedit /etc/apt/sources.list

修改为以下内容：

deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-updates main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-updates universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-updates multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-backports main restricted universe multiverse
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-security main restricted
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-security universe
deb http://mirrors.tuna.tsinghua.edu.cn/ubuntu-ports/ focal-security multiverse

# deb http://security.ubuntu.com/ubuntu xenial-security main

软件安装指南

安装 NoMachine

参考链接：NoMachine 下载页面

安装搜狗输入法

参考链接：搜狗输入法安装指南

安装虚拟屏

参考链接：CSDN 博客 - 虚拟屏安装教程

安装 ShellCrash
	1.	切换到 root 用户：

sudo -i

如果需要密码，请输入密码。

	2.	确保处于 bash 环境（如已处于可跳过）：

bash


	3.	执行安装脚本：

export url='https://fastly.jsdelivr.net/gh/juewuy/ShellCrash@master' && wget -q --no-check-certificate -O /tmp/install.sh $url/install.sh && bash /tmp/install.sh && source /etc/profile &> /dev/null


	4.	订阅链接：

