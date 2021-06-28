## IDE

开发最好是选择一个IDE进行开发。这里我推荐两款IDE进行选择：

### GoLand

这里是 jetbrains 家族提供的一款 Golang IDE。它是付费软件。个人版付费计划是：

| 年份 | 价格 |
|:---:|:---:|
| 第一年 | $89.00 |
| 第二年 | $71.00 |
| 第三年起 | $53.00 |

具体可参考该网址：https://www.jetbrains.com/zh-cn/go/buy/#personal?billing=yearly

## VSCode

这个是微软提供的一款开发工具，不仅仅支持 Golang，而且支持支持其他语言，需要安装 go 组件才可以。目前Golang的Vscode组件是由官方进行维护的。

中文版介绍地址：https://learnku.com/docs/go-blog/the-vs-code-go-plug-in-will-be-officially-maintained-by-go/8709

安装后，如果打开一个go文件去编辑的时候，右下角就会提示一些缺失的组件需要我们去安装，安装后就可以正常使用了。

这里的使用可以根据你的喜好和习惯来进行选择。

## 个人选择

有钱就上 Goland，没钱就上 VSCode。

## VSCode 配置

首先安装最新版本的 VSCode。

然后安装以下扩展：

- [`Go`](https://marketplace.visualstudio.com/items?itemName=golang.go)
    
> 安装该扩展后后续会安装一些命令，这里提示一下，最好按照上一页设置镜像那一节进行设置，否则你就会发现很多包都会安装失败了。

## 错误排查

- **Version of Go is too old for this version of Delve**

解决方案：

在非go项目中执行以下命令：

```bash
go get github.com/go-delve/delve/cmd/dlv
```