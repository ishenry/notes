# 配置maven及阿里云镜像
## 安装maven，设置环境变量
1. 下载maven安装包，解压到D:\Program Files\apache-maven-3.3.9
2. 新建系统变量MAVEN_HOME，变量值：D:\Java\apache-maven-3.3.9
3. 编辑系统变量Path，添加变量值：;%MAVEN_HOME%\bin
4. 在cmd窗口输入 mvn -version检测是否安装成功。

## 配置aliyun镜像
在D:\Program Files\apache-maven-3.3.9\conf\setting.xml文件中，找到<mirrors></mirrors>标签对。
添加aliyun镜像。效果如下：
```
<mirrors>
  <mirror> 
    <id>alimaven</id> 
    <name>aliyun maven</name> 
    <url>http://maven.aliyun.com/nexus/content/groups/public/</url> 
    <mirrorOf>central</mirrorOf> 
  </mirror>
</mirrors>
```
