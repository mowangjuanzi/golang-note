# 安装

## mac

首先安装 [`homebrew`](https://brew.sh/index_zh-cn) 。

接下来执行以下命令即可：

```bash
brew install golang
```

如果已经存在，则执行以下命令更新到最新版本

```bash
brew upgrade go
```

## Ubuntu

执行以下命令即可：

```bash
sudo apt install golang
```

如果更新到最新版本则执行：

```bash
sudo apt upgrade golang
```

## Windows

首先访问[Golang官网](https://golang.google.cn/dl/#featured) / [Golang 官方中国镜像](https://golang.google.cn/dl/) 获取下载地址。这里我使用的谷歌在国内制作的镜像网站。跟官网是同步的。可以看到顶部有四个推荐下载，我们选择 `Microsoft Windows` 块点击下载即可。

## 查看版本

使用以下命令查看版本：

```bash
% go version
go version go1.16.3 darwin/amd64
```

## Golang 包镜像

这样就安装好了。接下来还要做个事情，就是设置对 `package` 的镜像，因为很多都是都是拉取github 或者golang官网，因为需要翻墙的原因，我们需要设置镜像进行加速。这里我们使用了七牛云提供的镜像网站——[Goproxy中国](https://goproxy.cn/)：

```bash
go env -w GOPROXY=https://goproxy.cn,direct
```

这样安装就算是完成了。