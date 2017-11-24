Java程序，日志输出，我认为是第一位的，把它的应用拿到这里。

Spring-Boot对日志的处理，和我们往常的处理完全可以一致，通过logback.xml进行处理，即使有更先进的东西，我们也不用去管它。

这里，为了简便，我们任然使用前一篇的工程spring-boot-sample-data

第一步，在src/main/resources中增加logback.xml文件，文件内容为（这里仅最简单的，根据工程情况，进行相应的配置）：



```

```

注：1、控制台和日志文件的字符集

       2、日志文件的存放位置，须要遵守linux的命名规则

第二步，改造HelloController文件，改造结果如下



注：在添加引用时，日志的包一定是org.slf4j.Logger、org.slf4j.LoggerFactory



第三步、测试

1、运行程序

2、在浏览器中依次输入



http://localhost:8080/

http://localhost:8080/hello/上帝

3、在工程所在的根目录找到log文件夹，进去，再打开base.log，入下图

![](http://img.blog.csdn.net/20160624143453014?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)  


注：文件夹和日志文件的名称，都是在配置文件logback.xml中设置的

  


通过这个实例，我们完全用过去的技术处理日志，暂时不用去管别的，直接使曾经的技术。

