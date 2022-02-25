# kali安装docker环境

使用清华镜像，保证docker官网拉取的速度

```javascript
curl -fsSL https://mirrors.tuna.tsinghua.edu.cn/docker-ce/linux/debian/gpg | sudo apt-key add -
```

配置基于Debian版本的docker环境

```javascript
echo 'deb https://mirrors.tuna.tsinghua.edu.cn/docker-ce/linux/debian/ buster stable' | sudo tee /etc/apt/sources.list.d/docker.list
```

更新apt

```javascript
apt-get update
```

清除旧版本的docker

```javascript
apt-get remove docker docker-engine docker.io
```

安装docker

```javascript
apt-get install docker-ce
```

查看docker状态

```javascript
systemctl status docker
```

启动docker

```javascript
systemctl start docker
```

开机自动启动

```javascript
systemctl enable docker
```

安装docker-compose

```
apt-get install docker-compose
```

![image-20210121182541393](C:\Users\dell\AppData\Roaming\Typora\typora-user-images\image-20210121182541393.png)

见到版本安装成功

