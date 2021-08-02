# 解决rosdep update 的 timeout 问题

## 错误内容
之前执行``rosdep update``的时候，就报下面的错误，总的来说就是显示超时。

```shell
jingyl@jingyl-KLVC-WXX9:~/桌面/ROS_study$ rosdep update
reading in sources list data from /etc/ros/rosdep/sources.list.d
Hit https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/osx-homebrew.yaml
ERROR: unable to process source [https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/base.yaml]:
	<urlopen error [Errno 104] Connection reset by peer> (https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/base.yaml)
ERROR: unable to process source [https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/python.yaml]:
	<urlopen error [Errno 104] Connection reset by peer> (https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/python.yaml)
ERROR: unable to process source [https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/ruby.yaml]:
	<urlopen error _ssl.c:1114: The handshake operation timed out> (https://raw.githubusercontent.com/ros/rosdistro/master/rosdep/ruby.yaml)
Hit https://raw.githubusercontent.com/ros/rosdistro/master/releases/fuerte.yaml
Query rosdistro index https://raw.githubusercontent.com/ros/rosdistro/master/index-v4.yaml

ERROR: error loading sources list:
	<urlopen error <urlopen error [Errno 104] Connection reset by peer> (https://raw.githubusercontent.com/ros/rosdistro/master/index-v4.yaml)>
```
## 解决办法
