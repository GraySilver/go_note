## Hello World！

### 安装Go

Go支持以下系统

- Linux
- FreeBSD
- Mac OS X（也称为 Darwin）
- Window

安装包下载地址为：<https://golang.org/dl/>。

**UNIX/Linux/Mac OS X, 和 FreeBSD 安装**

1、下载源码包：go1.4.linux-amd64.tar.gz。

2、将下载的源码包解压至 /usr/local目录。

```shell
tar -C /usr/local -xzf go1.4.linux-amd64.tar.gz
```

3、将 /usr/local/go/bin 目录添加至PATH环境变量：

```shell
export PATH=$PATH:/usr/local/go/bin
```

**WIN下安装**

Windows 下可以使用 .msi 后缀文件直接安装，若安装目录在 C:\Go中，将 C:\Go\bin 目录添加到 PATH 环境变量中。添加后你需要重启命令窗口才能生效。

### 执行Go程序

1. 使用 go run 命令，直接在命令行输入 go run xxxx.
2. 使用 go install 编译程序，例如 go install hello，然后直接运行对应的hello程序即可。

### 编写Go脚本

```go
package main //每一个 Go 文件都应该在开头进行 package name 的声明(只有声明main时候是执行文件)

import "fmt" //导入包

func main() {
  
	fmt.Println("hello world") //print hello world.
}
```

