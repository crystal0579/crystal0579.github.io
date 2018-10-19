在eclipse里 project -> run configurations ->
里面有两个比较confused的东西， 
一。
enviorment 
它是操作系统级别的， 通过 system.getProperty("xxx")从os读到项目里
以windows为例， 它可以在操作环境变量里设置
也可以在 eclipse 里设置， 即 enviroment里设置，当然只有在eclipse启动才有效果， 但是项目容器绝对不能是, 某类的jvm 的main, 可以是tomcat等

二。
argument
它是jvm级别的， 只有在相关的jvm启动时才有效果， 需要我们在项目启动时设置相关的参数
可以是外部命令式 java -Dxxx=“xxx”
也可以在eclipse里的vm arguments里以 -D的方式设置


