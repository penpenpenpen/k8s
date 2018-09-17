#### 1.自己应用的部署

将代码通过GOOS=linux GOARCH=amd64 go build .进行编译生成二进制文件blog,将二进制文件通过Dockerfile文件打成镜像（docker build -t blogweb/images . ）通过deployment进行部署，server进行对外提供网络访问服务

#### 2. redis的部署

从镜像仓库拉去redis镜像，用deployment直接去部署，容器对外提供默认端口6379，service直接对外提供网络服务（这里是对自己的应用提供数据的增删改查服务），连接方式为ip+端口号
