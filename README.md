# ng-book2中文版反馈与勘误

## 随书源码

本书的随书源码位于 <https://github.com/ng-book2/code> 库中，可下载以供练习。

## 勘误

[点此添加新的勘误](https://github.com/ng-book2/book/issues?q=is%3Aissue)

全书 所有引用了angular.io文档的地方都可能由于防火墙原因而无法访问，只要把链接中的`angular.io`改为`angular.cn`即可访问对应的中文文档，不需要翻墙。（by 雪狼）

全书 如果你使用了最新版的`@angular/cli`，而不是书中所引用的`angular-cli`版本，请注意在创建项目时把项目名称中的所有下划线替换为中线，因为新版cli添加了更强的命名约束，不再允许出现下划线。如`ng new my_app`必须改为`ng new my-app`，否则会报错。（by [JonnBox](https://github.com/JonnBox)）

P#4 第一章第三行在学习本书时可以使用这个命令行安装angular-cli，但是在正式产品环境下建议使用`npm i -g @angular/cli`，因为官方已经推出了正式版，并且改了包名。命令行没变。（by 雪狼）

P#4 由于国内有防火墙的阻挡，因此安装可能会失败，如果发现`angular-cli`安装失败，请用`npm i -g cnpm`安装好[cnpm](https://cnpmjs.org/)，然后在全书中使用cnpm代替npm命令。（by 雪狼）

P#102 第4.7节 ngNodBindable拼写错误，应为ngNonBindable。（by Edward & [sanqianwdj](https://github.com/sanqianwdj)）

P#117 第5章中原书多处对Semantic UI的使用有误，请自行为这些表单定义样式来覆盖默认样式`.ui.form .error.message { display: block !important; }`，否则错误提示会永远看不见。此处只要用`*ngIf`控制可见性即可，不需要借助Semantic UI来隐藏。（by [lolhezihehe](https://github.com/lolhezihehe)）

P#220 第9章 上部多了一行重复的LocalStorage。（by 王子实）

P#221 第九章第二段 可观察对象 observable 英文首字母应该大写 Observable。（by [sanqianwdj](https://github.com/sanqianwdj)）

P#221 第九章提示部分排版失误 Flux一段应该同样是第一个列表的一部分。第一个列表中最后两段应合并为一段。（by [sanqianwdj](https://github.com/sanqianwdj)）

P#225 第四行应为“你可以点击会话和别人聊天”（原文为another people）。（by [sanqianwdj](https://github.com/sanqianwdj)）

P#365 列表第一行，`@inputs`注解应改为`@Input()`注解。（by 雪狼）

第7章 music应用中访问`https://api.spotify.com`接口会有跨域限制，修改如下：（by [twolun](https://github.com/twolun))
1. 新增`proxy.conf.json`配置文件
2. 修改package.json命令
  ```json
  "start": "ng serve --proxy-config proxy.conf.json",
  ```
3. 执行 ```npm start```

## 反馈

欢迎给我们[提issues](https://github.com/ng-book2/book/issues/new)

## 感谢有你！

（给我们提出纠错的书友们将来也会出现在这里）

网友 阿狸不歌 写了一篇读后感（上下篇），大家可以当做导读来看 <http://www.jianshu.com/p/9170620f772a> 、 <http://www.jianshu.com/p/1eb10ffb82e8>


