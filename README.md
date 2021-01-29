"# plazma-burst-2-website-css-rebuild"  
根据:  
https://www.plazmaburst2.com/?s=0&a=  
整出来的css，使用方法在html文件里按顺序引入fix.css和pb.css就可以用了  
index.html为demo，可以在里面看看样式咋用，一般是给div添加pb-XXXX的类就起作用了  
来自 超时空战士吧-317607692  

首先：  
在需要使用以下类时，需要在范围内的div先加pb-body，比如在body标签中  
常用：  
大的东西：
pb-body：没啥属性，以下的东西需要作用的话就在body加  
pb-header：官网头部，包含背景图  
pb-content：官网中部内容块，没啥属性  
pb-footer：官网底部，包含背景图  
中等大小的东西：
pb-container：官网首页用来放news，游戏，文章等等的面板，神tm他背景写死，虽然高度可以无限扩大，可是用的是背景图重复的操作，边框也是包含在背景图里的，所以目前只能固定宽度了。
小的东西：
pb-avatar：头像  
pb-link：超链接  
pb-level：头部右上角的等级（比如PROmoted）  
pb-pagination：分页器（官网这玩意做的真的简陋）  
pb-article-splitter：文章内的迷の分隔块  
pb-article-news-date：在官网news中，用于在每一条新闻开头中显示news更新的时间
pb-top-players：排行榜表格，在官网中用于显示前20名的玩家  

其他想说的：  
在pb-container中写文章，如果要引用b站视频播放器，需要给b站播放器的iframe添加一个bili-player的类，就可以以正常大小显示了（毕竟pb-container的宽度是固定死的）