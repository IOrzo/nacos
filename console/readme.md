# windows 启动时参数
-Xms512m -Xmx512m -Xmn256m -Dnacos.standalone=true -Dloader.path=F:\software\nacos-2.0.3/plugins/health,F:\software\nacos-2.0.3/plugins/cmdb -Dnacos.home=F:\software\nacos-2.0.3
 
# 根据上面参数，调整为 idea 参数
-Xms512m -Xmx512m -Xmn256m -Dnacos.standalone=true -Dnacos.home=G:/gitProjects/nacos/console

# conf/application.properties 设置 tomcat 日志目录
server.tomcat.basedir=G:/gitProjects/nacos/console

# conf 目录
conf 目录与发布包相对应，与 distribution 目录下一样的，这里是手动复制过来的

# 生成的目录
data、logs、目录是程序启动时自动生成的
