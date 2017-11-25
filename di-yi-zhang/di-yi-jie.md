另外在 v3 版本中引入了 part 的概念 \(通过标题或者水平分割线将 GitBook 分为几个 part\)，所以目录的索引格式为

`part-index + article-index`

。但是很多时候我们可能只有一个 part，并且不希望添加 part-index，即

`1.1`

,

`1.2`

-

&gt;

`1`

,

`2`

。官方说是会在 v4 版本中解决这个问题，如果 v3 版本中希望去掉前面的 part-index，需要我们手动修改 gitbook 的源文件，下面是修改方法：

