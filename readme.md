https://rocketmq.incubator.apache.org/docs/quick-start/

## Prerequisite
* 64bit OS, Linux/Unix/Mac is recommended;
* 64bit JDK 1.7+;
* Maven 3.2.x
* Git

Install maven
```bash
wget http://mirrors.hust.edu.cn/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz
```

修改环境变量，在/etc/profile中添加以下几行
```bash
MAVEN_HOME=/home/pdt_pa_zhangjun/apache-maven-3.3.9
export MAVEN_HOME
export PATH=${PATH}:${MAVEN_HOME}/bin
```
记得执行source /etc/profile使环境变量生效。

## Clone & Build
```bash
> git clone https://github.com/apache/incubator-rocketmq.git
> cd incubator-rocketmq
> mvn clean package install -Prelease-all assembly:assembly -U
> cd target/apache-rocketmq-all/
```

