## 你好，世界

这里我先编写一个简单的 `go` 文件，然后展示一下最基本的 `go` 文件到底是什么样的。

```golang
package main

import "fmt"

func main() {
	fmt.Println("hello world")
}

```

然后在当前目录下执行以下命令：

```bash
$ go run main.go
hello world
```

这里我们首先会认识到几个关键字，它们分别是 `package`, `import`， `func`。

## package

该指令主要是定义包的名字，默认包的名字是`main`。

## import

这里类似PHP的`use`或者Clang的`#include`。

用来引入我们需要调用的方法。

## func

这个代表我们定义的函数名称。

格式为 `func FuncName`，这里需要说明的一点是，Golang 没有类似面向对象的访问控制。只有一个，就是如果定义的方法名是大写开头，表示可外部访问的，否则就是外部不可访问的。所以看到我们调用的打印方法`Println`是`P`开头的。

## 总结

这里就先简单介绍一下最基本的，后面会进行更多详细介绍。