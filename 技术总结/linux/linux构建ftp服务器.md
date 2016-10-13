# linux 构建 ftp服务器

## 背景
linux下载东西非常麻烦， 很多时候想在windows下下好了，然后上传给Linux用， 这时候利用ftp就非常方便了。

## 搭建ftp服务器
linux下配置ftp服务器非常简单。

1. 安装 sudo apt-get install vsftpd。安装完毕以后会自动启动ftp服务
2. 配置 sudo vim /etc/vsftpd.conf, 设置其中 write_enable=YES
3. 重启ftp服务 sudo service vsftpd start | stop | restart
4. 检查ftp是否启动 netstat -tl

## 访问fpt服务器

首选须看查看本机的Ip是什么： ifconfig， 
然后可以：

1. 在浏览器中直接访问 ftp://192.168.20.129/
2. 使用 FileZilla 客户端

![](https://img.alicdn.com/imgextra/i2/46754672/TB2r_lhnXXXXXckXXXXXXXXXXXX_!!46754672.jpg)

