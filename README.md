# NLPBasic

## Word Embedding [note](https://github.com/wlyang538/NLPBasic/blob/main/Word_Embedding.md)


### Docker note： how to transfer file bewteen docker and local

- local to docker: docker cp /路径/文件名 容器ID:/上传路径 \
  for example: sudo docker cp gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabi.tar.xz 00e7d0f73704:/usr/share/
  
- docker to local: docker cp 容器ID:/上传路径 /路径/文件名 \
  for example: sudo docker cp 00e7d0f73704:/usr/local/arm/rootfs-debian/123.txt /usr/share/
  

### torch-scatter install

[install method](https://zhuanlan.zhihu.com/p/504134665)

### Docker push image to repo

- docker ps //查看镜像
- docker commit <exiting-Container> <hub-user>/<repo-name>[:<tag>] 将该容器生成镜像
- docker tag <existing-image> <hub-user>/<repo-name>[:<tag>] 如果存在镜像 tag 该镜像
- docker push<hub-user>/<repo-name>:<tag> 将镜像push到你的repo
