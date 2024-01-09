# Portainer-CN2021-IMNKS.COM

本Portainer界面汉化文件来源于CecOS CaaS容器云平台，版本:2.21.0：开源GPL 2.0协议

本站修改，测试Portainer 1.24.2使用OK，不支持Portainer CE，老、旧、弱、arm等机子建议用这个

1、下载汉化文件，解压出public文件夹 2、举例把文件夹传输至系统root目录（自行修改） 3、然后按需执行以下命令

## docker run

docker volume create portainer_data

docker run -d -p 9000:9000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /root/public:/public portainer/portainer:latest
