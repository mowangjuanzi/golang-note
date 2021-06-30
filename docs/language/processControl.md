# 流程控制

- if else

```go
if num := 2; num > 2 {
	fmt.Println("false")
} else if num == 2 {
	fmt.Println("true")
} else {
	fmt.Println("null")
}
```

这里可以看到，跟其他语言的 `if-else` 几乎没有什么差别。但是跟PHP相比，最重要的是if的判断值必须是bool值。

- switch

```go
switch num := 1; num {
case 1:
    fmt.Println("星期一")
case 2:
    fmt.Println("星期二")
case 3, 4:
    fmt.Println("星期三四")
default:
    fmt.Println("null")
}
```

- for
- range
- goto
- break
- contine