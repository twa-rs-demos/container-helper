# Container Helper Script

修改 `container` 第三行
```
cd /home/afaren/twars/assembly
``` 
中的项目路径为你 recruiting-system 的路径，比如
```
cd /home/workspace/recruiting-system/assembly
```

并**将文件 `container` 放置到系统可执行文件路径之下**，即可使用。


想要启动的容器，只需要在 container start 后面跟上容器名即可，用法可以参考 `docker-compose`, 比如
```
$ assembly/ docker-compose up -d
$ assembly/ docker-compose up -d mysql 
$ assembly/ docker-compose up -d mysql paper-api 
```

使用 `container`，你就**可以在任意目录下启动容器**，不需要特意跑到 `assembly` 目录下

```
$ container start			
$ container start mysql  
$ container start mysql paper-api 

```

停用容器也是一样的做法：
```
$ container stop		
$ container stop mysql  
$ container stop mysql paper-api 

````
