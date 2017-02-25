# samba - 文件共享服务

site : https://www.samba.org/

Samba是Ubuntu和Windows进行网络共享的工具，比如分享打印机，互相之间传输资料文件。

## 安装Samba

> `sudo apt-get install samba`

## 配置samba

> `sudo gedit /etc/samba/smb.conf`

```
[share]
	comment = share folder
	path = /home/user/share_folder
	writeable = yes
	guest ok = yes
```

如果不想让匿名用户也可以在服务器上写文件，
将 writeable 值写为 no .

如果完全不想让匿名用户访问，
将 guest ok 值写为 no .

## 添加samba用户

如果samba的配置文件上写着guest ok = yes，那么匿名用户是不需要帐号密码就可以访问
samba服务的。否则就要使用samba帐号登陆samba服务。

在samba服务器上建立samba帐号的步骤如下： 

1. 在samba服务中添加linux用户，用户名为user
> `smbpasswd -a user`

2. 激活samba用户,用户名为user
> `smbpasswd -e user`

## 在ubuntu 14.04 上访问 samba 服务

在 shell 中输入以下命令
> nautilus-connect-server