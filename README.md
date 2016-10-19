# RankChart
一个展示排名的图标插件
* 支持自动排序
* 支持加载动画提示
* 支持改变数据

## 使用方法

* 引入`ranking-chart.css`,`ranking-chart.js`文件
``` html
<link type="text/stylesheet" src="ranking-chart.css"></link>
<script type="text/javascript" src="ranking-chart.js"></script>

```
* 编写html文件
``` html
<!--在html里面定义一个div作为显示容器-->
<div id="rank-chart" class="rank-chart"></div>

```
* 编写javascript文件
``` javascript
// 实例化组件
rc = RankingChart(container,
            day_rank,
            {
                titleTxt: '日排行名',
                titleTxtColor: '#197EE8',
                titleColor: 'gainsboro',
                itemNoBgColor: '#F5E401',
                itemNoColor: 'black',
                itemNameColor: '#24ADFF',
                itemBarColor: '#B1D6FF',
                itemValueColor: 'black'
            });

// 改变数据前加载动画
rc.perLoading（）

// 改变数据
rc.changeData(data,settings);

```
## 参数说明

* titleTxt: 标题名称,
* titleTxtColor: 标题名称颜色,
* titleColor: 标题背景颜色,
* itemNoBgColor: 排行表条目标号背景颜色,
* itemNoColor: 排行表条目标号字体颜色,
* itemNameColor: '排行表条目名称字体颜色',
* itemBarColor: 排行表条目数值所占比例条颜色,
* itemValueColor: 排行表条目数值字体颜色

## api说明

* perLoading: 加载数据动画
* changeData: 改变数据内容

## 效果
![image](https://github.com/kuangch/RankChart/blob/master/ranking-chart.gif)
