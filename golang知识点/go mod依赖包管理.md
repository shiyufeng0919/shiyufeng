# go mod 依赖包管理

## 一. go mod 常用命令



```linux
$ go mod help #查看帮助
$ go mod tidy #根据go.mod文件来处理依赖关系
$ go mode download #下载依赖
$ go mode vendor #将依赖包复制到项目的vendor目录。方便用户快速使用命令 go build -mod=vendor 编译
$ go list -m all #显示依赖关系。
$ go list -m -json all #显示详细依赖关系
```

