mvn创建项目
1.mvn archetype:generate -DgroupId=com.hand  -DartifactId=test1  -DarchetypeArtifactId=maven-archetype-quickstart  -DinteractiveMode=false

-DarchetypeCatalog=local（然后在执行的命令后面加上增加参数-DarchetypeCatalog=local，变成读取本地文件即可。）
会默认下载到用户名.m2文件夹
2.mvn clean compile

3.mvn clean compile  exec:java -Dexec.mainClass="com.hand.App" -Dexec.args="arg0 arg1 arg2"

4.mvn exec:java -Dexec.mainclass="com.hand.App" -Dexec.args="arg0 arg1 arg2"

maven创建Web项目
mvn archetype:generate -DgroupId=com.hand -DartifactId=webtest -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

-DarchetypeCatalog=local（然后在执行的命令后面加上增加参数-DarchetypeCatalog=local，变成读取本地文件即可。）

mvn clean 项目名称
运行 mvn jetty:run
