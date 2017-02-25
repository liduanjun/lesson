# Install Ubuntu 14.04 amd64

## Download Ubuntu

[MainSite](http://mirrors.ustc.edu.cn/) ->
[Ubuntu 14.04 amd64 ISO](http://mirrors.ustc.edu.cn/ubuntu-releases/14.04.4/ubuntu-14.04.4-desktop-amd64.iso)

## Copy Ubuntu to USB flash drive

In ubuntu 
> * Startup Disk Cteator (ubuntu live自带有)

In Windows
> * UltraISO
> * [ImageWriter](http://cloud.github.com/downloads/openSUSE/kiwi/ImageWriter.exe)

## Install Ubuntu
> 1. boot pc , press key f12 , chioce usb flash driver
> 2. next->language,timezone,disk,account->...
> 3. reboot

## Confige Ubuntu

### confige source

[ustc](https://mirrors.ustc.edu.cn/repogen/)

> gedit /etc/apt/source.list

```
deb http://mirrors.ustc.edu.cn/ubuntu/ trusty main restricted universe multiverse
deb-src http://mirrors.ustc.edu.cn/ubuntu/ trusty main restricted universe multiverse
deb http://mirrors.ustc.edu.cn/ubuntu/ trusty-security main restricted universe multiverse
deb-src http://mirrors.ustc.edu.cn/ubuntu/ trusty-security main restricted universe multiverse
deb http://mirrors.ustc.edu.cn/ubuntu/ trusty-updates main restricted universe multiverse
deb-src http://mirrors.ustc.edu.cn/ubuntu/ trusty-updates main restricted universe multiverse
deb http://mirrors.ustc.edu.cn/ubuntu/ trusty-backports main restricted universe multiverse
deb-src http://mirrors.ustc.edu.cn/ubuntu/ trusty-backports main restricted universe multiverse
```

### config proxy

[shadowsocks-wiki](https://github.com/shadowsocks/shadowsocks-qt5/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)

> sudo add-apt-repository ppa:hzwhuang/ss-qt5  
> sudo apt-get update  
> sudo apt-get install shadowsocks-qt5  

### config proxychains

> sudo apt-get install proxychains  
> gedit /etc/proxychains.conf

```
http 127.0.0.1 1008
```

### config vscode

[MainSite](https://code.visualstudio.com/)

```
dpkg -i code_xxx.deb
```

### config samba

> sudo apt-get install samba

```
[liduanjun]
   comment = liduanjun's share folder
   path = /home/ldj/share
   guest ok = yes
   browseable = yes
   writable = yes
   create mask = 0755
```