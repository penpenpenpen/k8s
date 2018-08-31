# k8s
本代码用dockerfile构建自己的镜像，通过deployment对镜像做部署，通过service对外提供服务

在编译自己的代码是需要使用GOOS=linux GOARCH=amd64 go build 代码名
在构建dockerfile文件时使用sudo docker build -t 镜像标签名 指定dockerfile所在的路径（如果为当前路径使用 . ）
