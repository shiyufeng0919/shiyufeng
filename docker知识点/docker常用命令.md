# Docker常用命令汇总

## docker镜像



## docker启动容器

```linux
#启动容器,退出容器，则删除该容器
$ docker run -it --rm --name 容器名称 --entrypoint=bash 镜像ID
```

## docker tar包

```linux
#通过docker save将镜像保存为文件(归档文件)
$ docker save -o 归档文件名.tar 镜像ID 

#将多个镜像保存为tar文件
$ docker save -o 归档文件名.tar 镜像ID1 镜像ID2

#导入保存的镜像(即将tar中的镜像导入到docker中)
$ docker load -i 归档文件名.tar
或
$ docker load --input 归档文件名.tar
```

## docker cp

```linux
#从宿主机拷备文件到容器中
$ docker cp 目标文件 容器名:容器目录   #eg: docker cp ledger.init lrtmc-jdchain:/usr/local/peer

#从容器拷备文件到宿主机
$ docker cp 容器名:容器文件 宿主机目录 #eg: docker cp lrtmc-jdchain:/usr/local/peer .
```

## Dockerfile制作镜像

## docker-compose启动容器

