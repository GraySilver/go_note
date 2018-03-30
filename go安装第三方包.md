### Go安装第三方包

由于自己需要安装一个MySQL第三方包，例如：  http://github.com/go-sql-driver/mysql

找了挺多教程没有一个很好的讲述，终于看到一个解决方法，整理一下放在此处。

#### 设置Gopath

1、Window上设置

右键我的电脑——高级系统设置——环境变量，系统变量下 点击【新建】

输入：   

- 第1行：GOPATH    
- 第2行：你指定路径，例如: D:\go\gopath  

2、安装git for windows

下载地址：http://git-for-windows.github.io/

 3、之后执行命令安装第三方包

```shell
go get github.com/go-sql-driver/mysql
```

这条命令它会把类库包源代码，下载解压到你的 %GOPATH% 路径里面去。
比如：D:\go\gopath\src\github.com\go-sql-driver\mysql

4、执行可以在gopath中看到对应的库，证明下载成功。

#### Reference

https://studygolang.com/articles/5840