# Flysoloing Maven Repository

##  如何使用？

1. 首先复制如下配置代码，分别为libs和plugins
```xml
<repositories>
    <repository>
        <id>flysoloing-maven-libs-repo</id>
        <name>Flysoloing Maven Libs Repository</name>
        <url>http://flysoloing.github.io/repo/libs</url>
    </repository>
</repositories>
```
```xml
<pluginRepositories>
    <pluginRepository>
        <id>flysoloing-maven-plugins-repo</id>
        <name>Flysoloing Maven Plugins Repository</name>
        <url>http://flysoloing.github.io/repo/plugins</url>
    </pluginRepository>
</pluginRepositories>
```

2. 然后设置第三方远程仓库，有两种方式：

* 全局配置，在`~/MVN_HOME/conf/settings.xml`中，找到`<profiles>...</profiles>`，作为profile添加
* 局部配置，在需要使用插件的应用代码中，找到`pom.xml`，粘贴步骤1配置代码