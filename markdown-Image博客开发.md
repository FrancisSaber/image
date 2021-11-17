vuepress，引入script文件

在.vuepress 的config的head中引入

#### vue引入外部js压缩文件不能被使用的问题

vue引入jq以及zepto之类的压缩文件是直接一个$变量名就可以使用的，但是有一些压缩的js并不可以像jq一样直接在vue内部使用的

某些js文件要在index.html里用`script`标签引入

#### <font color="orange">在JS文件引入无法直接import 导入或者 require导入的文件 </font>

```js
index.js
(function(){
    //js创建script标签 引入目标js文件
    document.write("<script language=javascript src="+'https://cdn.jsdelivr.net/gh/litstronger/live2d-moc3@master/js/l2d.js'+"></script>");
})()

export default 函数方法/类
```

