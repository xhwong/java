## 获取jdk源码

+ 源码地址：[http://hg.openjdk.java.net/](http://hg.openjdk.java.net/)

+ 获取代码的方式：版本控制工具使用的是Mercurial
    + 安装方式参考：[https://www.mercurial-scm.org/wiki/Download](https://www.mercurial-scm.org/wiki/Download)
+  mac 下可以直接：

```
    brew install mercurial
```

![image](https://user-images.githubusercontent.com/18548200/68681965-527bb780-059f-11ea-89ee-a19f4ea723a2.png)

    
+ 安装之后，开始下载源码： 

```
hg clone http://hg.openjdk.java.net/jdk8/jdk8 
```

+  cd YourOpenJDK：
> 目录如下所示
 + ![image](https://user-images.githubusercontent.com/18548200/68683852-7a204f00-05a2-11ea-8ab1-fe46185f84b3.png)

     
+  开始下载：
```
sh ./common/bin/hgforest.sh clone "$@" || exit 1
```
> 下载完成之后自动停止。至此jdk代码下载完毕

+ 更新代码

```
sh ./common/bin/hgforest.sh pull -u
```


