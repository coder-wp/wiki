打开tomcat安装目录下的conf目录下的server.xml，在host标签里添加如下内容：

`<!-- 去掉项目名 -->`

` <Context path="" docBase="projectName" reloadable="true" />  `

![](/assets/tomcat-server.png)

