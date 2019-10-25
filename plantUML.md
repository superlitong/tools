
#Windows系统下vs code安装plantUML插件

#前置需求

Java
graphviz
vs code

#安装java并为其配置环境变量,java/javac检测是否成功

变量名：JAVA_HOME
变量值：C:\Program Files (x86)\Java\jdk1.8.0_91        // 要根据自己的实际路径配置
变量名：CLASSPATH
变量值：.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;         //记得前面有个"."
变量名：Path
变量值：%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;


#安装graphviz并配置环境变量，dot -version 检测是否成功

变量名：GRAPHVIZ_DOT
变量值：C:\Program Files (x86)\Graphviz 2.28\bin\dot.exe        // 要根据自己的实际路径配置


#在vs code中直接搜索，并安装plantUML插件

设置-扩展-PlantUML配置，Java可执行文件位置填写：C:\Java\jdk13\bin\java.exe    // 要根据自己的实际路径配置
打开UML文件，按ALT + D 即可实时预览UML图

