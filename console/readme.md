# windows 启动时参数
-Xms512m -Xmx512m -Xmn256m -Dnacos.standalone=true -Dloader.path=F:\software\nacos-2.0.3/plugins/health,F:\software\nacos-2.0.3/plugins/cmdb -Dnacos.home=F:\software\nacos-2.0.3
 
# 根据上面参数，调整为 idea 参数
-Xms512m -Xmx512m -Xmn256m -Dnacos.standalone=true -Dnacos.home=G:/gitProjects/nacos/console -Dspring.profiles.active=dev

# 配置文件
与直接下载的打包文件相比，conf 目录配置文件在 distribution 项目目录下，将配置文件复制一份到 resources 目录下，改名为 application-dev.properties，方便自己对项目配置

# application-dev.properties 设置 tomcat 日志目录
server.tomcat.basedir=G:/gitProjects/nacos/console
server.tomcat.accesslog.directory=G:/gitProjects/nacos/console/logs

# 生成的目录
data、logs、目录是程序启动时自动生成的

# consistency 项目
consistency 项目中使用了 protobuf，在启动前需先将该项目编译
