
# 使用Hugo搭建静态文件管理系统

# hugo介绍
Hugo是由Go语言实现的静态网站生成器。 注意试试生成器。他虽然自带webserver，但是只是为了方便本机调试（对比nginx没做）。 他能非常方便的把markdown文件转换为html。

#使用

1. 创建站点： hugo new site  hub_site
2. 创建一个 about 页面: hugo new about.md
3. 创建第一篇文章，放到 post 目录：hugo new post/first.md


## 安装皮肤
 	
	cd themes
	git clone https://github.com/spf13/hyde.git


##启动服务

	hugo server --theme=hyde --buildDrafts -p 80 --bind 115.28.83.94 -b http://115.28.83.94

注意 -b参数，如果不加这个，所有的资源文件的前缀都是localhost
	
也可以打包生成今天文件：

	hugo -t hyde -b http://115.28.83.94