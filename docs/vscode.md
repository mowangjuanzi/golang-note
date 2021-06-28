## VS Code 

在阅读本章前，请新确定已经按照前面的章节进行了相关的设置。

## 断点调试

具体的实践方法我就不说了。下面直接说如何实现吧。

手下，我们创建文件 `.vscode/launch.json`

填入以下内容：

```json
{
    // 使用 IntelliSense 了解相关属性。 
    // 悬停以查看现有属性的描述。
    // 欲了解更多信息，请访问: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "运行go",
            "type": "go",
            "request": "launch",
            "mode": "debug",
            "program": "${file}"
        }
    ]
}
```

参考内容：https://github.com/golang/vscode-go/blob/master/docs/debugging.md

## 未完待续

对于vscode，如果有什么疑问，可以给我提ISSUS。我会尽力进行解答。