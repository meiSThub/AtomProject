# 一、编译错误解决

更新到Android Studio 2020.3.1 版本后，创建新项目后，编译报错：

![image-20210910112659573](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210910112659573.png)	

查看了一下[官网Android Studio 和 AGP更新](![](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210910112848786.png))的信息，了解到，Android Studio Arctic Fox  2020.3.1 默认使用的是 Java 11：

![image-20210910112848786](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210910112848786.png)

所以，首先检查 build.gradle 配置信息，看使用的 Java 版本是否是 Java 11 版本，如果不是，则改成 Java 11，如：

![image-20210910113234756](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210910113234756.png)

如果编译还是报错，则查看Project 的设置信息，看使用的 Java 版本是否是 11，如果不是，则改成 java 11，如：

![image-20210910112536312](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210910112536312.png)

经过上面两个修改，基本上就可以编译通过了。

如果还报错，则检查buidl.gradle 配置是否正确，混淆配置项是否合法，如：

![image-20210927111857964](https://gitee.com/meiSThub/BlogImage/raw/master/2020/image-20210927111857964.png)

自动格式化成这样，是不符合语法要求的，需要保持一行。

总结：

* 修改工程的Java版本为 Java 11
* 修改build.gradle 中的Java 编译版本为 Java 11
* 检查其他配置是否正确，是否被格式化了。

# 二、更新差异

仔细对比，可以看到 ，AGP 7.0 之后，build.gradle 的配置项名称有一些变化，如：

| AGP 7.0 之前      | AGP 7.0 之后 |
| ----------------- | ------------ |
| compileSdkVersion | compileSdk   |
| minSdkVersion     | minSdk       |
| targetSdkVersion  | targetSdk    |

虽然在AGP 7.0 之后，字段名变化了，但还是可以使用原来的字段名。

