# CDYHomework
用来交作业的地方，我是17数新的CDY
<details>
<summary>Week1</summary>
<pre><code>
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

</code></pre>
</details>
<details>
<summary>Week2</summary>
<pre><code>
10月9日</br>

问题2</br>
国内政府的</br>
《上海市公共数据开放暂行办法》[上海市人民政府网站](http://www.shanghai.gov.cn/nw2/nw2314/nw2319/nw12344/u26aw62638.html)</br>
《中华人民共和国政府信息公开条例》 [百度律师/法律智库[(https://duxiaofa.baidu.com/detail?searchType=statute&from=aladdin_28231&originquery=%E6%94%BF%E5%BA%9C%E4%BF%A1%E6%81%AF%E5%85%AC%E5%BC%80%E6%9D%A1%E4%BE%8B2019&count=56&cid=27bf8b3a94630d68e58719938ec39bba_law)</br>
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
结果及检验请见文件 [同比增速.xls](https://github.com/RRC-c/CDYHomework/blob/master/%E5%9B%BD%E5%AE%B6%E7%BB%9F%E8%AE%A1%E5%B1%80GDP/%E5%90%8C%E6%AF%94%E5%A2%9E%E9%80%9F.xls)  </br>
</code></pre>
</details>
<details>
<summary>Week3</summary>
<pre><code>
10月16日
我使用了图表秀、百度图说、Tableau、Excel这4种工具
我选择的数据集是Kaggle上的 [自然资源部网站](http://www.mnr.gov.cn/gk/tzgg/201009/t20100915_1990379.html)[Steam_10_09_18_best_game](https://www.kaggle.com/michau96/steam-10-09-18-best-game)
