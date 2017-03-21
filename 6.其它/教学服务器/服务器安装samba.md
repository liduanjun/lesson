# 服务器安装 Samba

6.给服务器增加共享服务
    * 安装 samba
        * sudo apt-get install samba
    * 配置 samba 为个人(用账号)服务器
        * sudo vi /etc/samba/smb.conf
    * 文件末尾添加如下内容
        [t folder]
        comment = a share folder for everyone
        path = /home/t/t
        writeable = yes
        valid users = t # 这样这个目录只能被用户 t 访问
    * 重启smbd服务
        sudo service smbd restart
    * 重启客户端(笔记本)
        因为客户端存放着上次登陆的信息，如果不重启，就看不到samba配置文件更改的效果
    * 配置 samba 为共享(匿名)服务器
        * sudo vi /etc/samba/smb.conf
        * 建立一个目录当共享目录
            mkdir /home/t/share
            chmod 777 share
        * 文件末尾添加如下内容
            [share folder]
            comment = a share folder for everyone
            path = /home/t/share
            public = yes
        * 重启 smbd
            sudo service smbd restart
        * 如果要匿名可以给共享文件夹写文件，还需要在smb.conf加入
            comment = a share folder for everyone
            path = /home/t/share
            public = yes
            writeable = yes
        * 重启 smbd
            sudo service smbd restart
