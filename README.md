# CDYHomework
用来交作业的地方，我是17数新的CDY
<details>
<summary>Week1</summary>
9月30日
记录了一天的饮水情况，包括饮水的时间、容器/饮料种类、每次饮水量（用吞咽数测量）。我从9月26日中午开始记录，直到9月29日凌晨结束。

可视化是我用数位板手绘完成的，限于精力，只绘制了第一天（9月26日下半天和9月27上半天）的记录（见9.26PM.jpg和9.27AM.jpg）。每张图以表盘呈现12小时的记录，每个节点用图标表示饮用的水的种类（详见图例），每个区段的颜色呈现的是：每次饮水后直到下一次饮水前我的“水含量”（见key.jpg），具体等于当此饮水吞咽数/直到下次饮水的小时数（记录见喝水情况表.xlsx）。

![image](https://github.com/RRC-c/CDYHomework/raw/master/Pics/9.26PM.jpg)</br>
![image](https://github.com/RRC-c/CDYHomework/raw/master/Pics/9.27AM.jpg)</br>
![image](https://github.com/RRC-c/CDYHomework/raw/master/Pics/key.jpg)

回答问题：

数据记录记录请见https://github.com/RRC-c/CDYHomework/blob/master/%E5%96%9D%E6%B0%B4%E6%83%85%E5%86%B5%E8%A1%A8.xlsx

感想：统计喝水这样的数据真的很繁琐，我觉得我这种可视化的形式可以用在一些智能水杯的app里—————当然就不需要用吞咽数计量了，可以更加精确。让一天的喝水情况直接可见————最好配一个“提醒喝水小助手”，感觉对生活还挺有帮助！

我的哪些个人数据被收集？被谁收集？答：日常的搜索记录————最明显的是淘宝————不光我在淘宝上的搜索，显然我平常的浏览器搜索数据都被淘宝收集到了。除此之外，我长期的或实时的地理位置显然被收集了————网页侧边栏出现我家乡的房地产广告/人才招聘广告，有时候也有我实时所在地的————不知道是谁在收集，推测应该是百度搜索引擎出卖了我。

</details>
<details>
<summary>Week2</summary>
10月9日</br>

问题2</br>
国内政府的</br>
《上海市公共数据开放暂行办法》[上海市人民政府网站](http://www.shanghai.gov.cn/nw2/nw2314/nw2319/nw12344/u26aw62638.html)</br>
《中华人民共和国政府信息公开条例》 [百度律师/法律智库](https://duxiaofa.baidu.com/detail?searchType=statute&from=aladdin_28231&originquery=%E6%94%BF%E5%BA%9C%E4%BF%A1%E6%81%AF%E5%85%AC%E5%BC%80%E6%9D%A1%E4%BE%8B2019&count=56&cid=27bf8b3a94630d68e58719938ec39bba_law)</br>
《政务信息资源共享管理暂行办法》[中国政府网](http://www.gov.cn/zhengce/content/2016-09/19/content_5109486.htm)</br>
《国土资源数据管理暂行办法》[自然资源部网站](http://www.mnr.gov.cn/gk/tzgg/201009/t20100915_1990379.html)</br>
还有地震局、气象局各种环境、科学数据的共享条例，不再列举</br>
国外的： </br>
美国 https://data.gov</br>
日本 http://www.data.go.jp/</br>
俄罗斯 http://opengovdata.ru/</br>
……</br>

问题3</br>
本意想算个同比数据，选取2011—2018年每一季度的“国内生产总值（不变价）当季值”为指标。 </br>
![image](https://github.com/RRC-c/CDYHomework/blob/master/%E5%9B%BD%E5%AE%B6%E7%BB%9F%E8%AE%A1%E5%B1%80GDP/%E9%A1%B5%E9%9D%A2%E6%88%AA%E5%9B%BE.png)</br>
算式：季度同比增速=（当季值-上一年同季值）/上一年同季值*100%  </br>
不变价已经去除了物价影响，理论上这就是同比增速。 </br>
但实际计算中出现了问题——2016年数据存在突出值，增速竟然达到20%以上！ </br>
这一计算方法是错误的。 </br>
原因在于物价的修正值前后有别，统计局的数据报表有注如下： </br>
"不变价数据按不同基期分段计算。其中，2011-2015年数据按2010年价格计算，2016年及以后各季度数据按2015年价格计算。累计数据由当季数据相加得到。" </br>
这就没法算了，我对照官方同比增速的数据做检验（官方同比增速用国内生产总值指数当季值做指标，算式：季度同比增速=指数当季值/100-1） </br>
发现除了极端值，其他数据也略有不同——这说明它们是用另外一个物价标准来修正的；这就触及我的知识盲区了，可能有待找一下物价方面的数据，目前还没找到正确方法。 </br>
结果及检验请见文件 [同比增速.xls](https://github.com/RRC-c/CDYHomework/blob/master/%E5%9B%BD%E5%AE%B6%E7%BB%9F%E8%AE%A1%E5%B1%80GDP/%E5%90%8C%E6%AF%94%E5%A2%9E%E9%80%9F.xls)   
</details>
<details><summary>Week3</summary>

10月9日  
我使用了图表秀、百度图说、Tableau和Excel四种工具  
用以呈现Kaggle上的数据集[Steam 10 09 18 best game](https://www.kaggle.com/michau96/steam-10-09-18-best-game)  
这个数据集为2018年9月10日steam上百大“best game”的当前在线人数（Now_Players）与24小时内的在线人数峰值（Best_Of_24）  
据此我们可以看到寥寥几个大型在线多人游戏压倒性的用户数量优势；如果仔细观察，也可以看出：比起单机游戏，在线多人游戏的峰值人数往往与当前游戏人数差别更大。  
**图表秀**  
![image](https://github.com/RRC-c/CDYHomework/blob/master/Pics/steam18-9-10%20best%20game%EF%BC%88%E5%9B%BE%E8%A1%A8%E7%A7%80%EF%BC%89.png)  
体会：*比较方便、功能不少的网页版可视化工具。图的种类很多，编辑字段、格式都很方便，给的几个配色模板也还挺漂亮。唯一不足就是作为网页版，导入数据和在有数据的情况下换图表是真的卡，卡死浏览器好几次。*  
**百度图说**  
![image](https://github.com/RRC-c/CDYHomework/blob/master/Pics/steam18-9-10%20best%20game%EF%BC%88%E7%99%BE%E5%BA%A6%C2%B7%E5%9B%BE%E8%AF%B4%EF%BC%89.png)  
体会：*百度图说更具排版工具的特点——它可以按页面编排多个图表，但它的可视化功能受限严重，太过轻量化，无法显示详细、文本密集之处。我用的数据集在图说就显示不出完整的坐标字段，导出的图片也分辨率不高。如果是简单的、仅仅是为辅助一些文本的图例我觉得可以用百度图说快速完成，其他情况下我认为这绝不是一个使用体验很好的可视化工具。*  
**Tableau**  
[点此查看pdf](https://github.com/RRC-c/CDYHomework/blob/master/Pics/steam18-9-10%20best%20game%EF%BC%88tableau%EF%BC%89.pdf)  
体会：*上手花了些时间，可以看出这是真正功能强大的可视化软件。但格式可以调整的地方有些少，而且免费版不能导出图片（差评）。还有一点，很多UI太集成了或者太简单了，我觉得右键可以点开有选项的地方，点开一看发现啥也没有，有点新手不友好。*  
**Excel**  
[点此查看pdf](https://github.com/RRC-c/CDYHomework/blob/master/Pics/steam18-9-10%20best%20game%EF%BC%88excel%EF%BC%89.pdf)  
体会：*体验完上面几个，才意识到excel是一个多么强大而便利的可视化工具。*  

</details>
<details><summary>Week4</summary>
  
10月29日  
*严格来讲这不是一篇新闻，这只能算一个科普小片段：*  
**白色污染泛滥，塑料包装或是最大祸首**  
塑料已经成为现代世界应用最广的人造材料，几乎从诞生之初人们就很关注它对环境的影响。塑料在生产生活中庞大的产量和使用量，以及其难以自然降解等特征给世界环境带来巨大压力。而2017年7月加州大学与佐治亚大学的一项研究显示：比起其他规模化生产的工业门类，包装产业使用塑料最多，同时它也成为产生最多塑料废料的产业。以2015年的数据为例：  
![image](https://github.com/RRC-c/CDYHomework/blob/master/Pics/Plastic-waste.jpg)  
与塑料总产量屈居第二的建筑产业不同，包装产业在大量运用塑料的同时产生塑料废料的比例相当之高，达到了惊人的97%。导致其废料泛滥的最大原因显然是塑料包装短暂的寿命。大多数塑料包装都属于一次性包装，一旦拆开就成为废料。研究指出，包装产业塑料产品的平均寿命只有半年，在所有门类的产品中垫底。而位列倒二的一般消费品（消费者与机构）平均也有3年的寿命。  
![image](https://github.com/RRC-c/CDYHomework/blob/master/Pics/Plastic-lifetime.jpg)  
除了短命这一最大原因外，比起交通、建筑等门类，包装产品在材料和形制上更具多样化，这给其回收利用带来困难。  
要缓解塑料废料给地球环境带来的压力，我们就不能回避塑料包装的问题。对于制造商和消费者来说，减少塑料包装的使用，选择便于回收、降解的塑料包装，支持垃圾分类，都有助于改善当前状况。而政府决策者需要更精细的管控经济产业的环境影响，积极运用立法手段改变现状。


过程与思路：  
数据主要来源于Roland Geyer1, Jenna R. Jambeck2 and Kara Lavender Law于2017年7月发表的研究[Production, use, and fate of all plastics ever made](https://advances.sciencemag.org/content/3/7/e1700782)，我所使用的3个数据集都是在Our World in Data网站上获得的，都可在[Plastic Pollution](https://ourworldindata.org/plastic-pollution)这一页面中下载。  
过程中还参考了转载在CSDN上的[Data Discovery:Global Plastic Waste](https://tduan.netlify.com/post/data-weekend-global-plastic-waste/)  
我获取的原始数据集是2015年各工业门类的塑料产量、2015年世界各工业门类塑料废料产生量和研究估算出的各门类产品平均寿命。  
Our World in Data本身分别在这几个数据集下提供了条形图。一开始我只是希望通过我的可视化体现各门类产生的塑料、塑料废料的比例关系，所以我选用饼状图。但这样显然太简单了，也没有新意，所以我回去看了网站数据来源的这篇研究。我最终决定呈现不同工业门类塑料产量和其废料生产量的比例关系——这意味着这个门类是否是个浪费塑料的产业。所以我最后想出一个有点类似一个饼状图+一个南丁格尔图的可视化方案，表示两重比例。由于扇形面积表示的比例不是直观的（半径应是所表示比例的平方根），所以我给小一级的比例（废料产生量/塑料产量）在图上做了标明。  
原研究中对这个比例的论述是建立在他们对塑料产品寿命的研究上的，为了说明高废料比例背后的原因，我补充了产品平均寿命的数据，做出了第二张图。  
两张图都是用可视化工具（第一张是图表说，第二张是tableau）制作雏形后转入ps加工成的，而第一张图中小一级比例（废料产生量/塑料产量）的扇形/小扇形，则是经过计算后在ps上单独画出的。

</details>
