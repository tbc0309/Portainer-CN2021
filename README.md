# Portainer-CN2021-IMNKS.COM

本Portainer界面汉化文件来源于CecOS CaaS容器云平台，版本:2.21.0：开源GPL 2.0协议

1、下载汉化文件，解压到public文件夹 2、文件夹传输至系统根目录 3、然后按需执行以下命令

## x86-64系统使用

docker volume create portainer_data

docker run -d -p 9000:9000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer

## ARM64系统使用

docker volume create portainer_data

docker run -d -p 9000:9000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:linux-arm64
