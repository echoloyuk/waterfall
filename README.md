# Waterfall

极其简单的瀑布流组件。
![demo](./doc/demo.png)

使用该组件需要注意：
* 每一个瀑布流元素的宽度必须相同。
* 不支持动态布局。每次元素的宽度或数量变更需要重新执行方法。
* 瀑布流容器宽度不能改变。

# 使用方法

它非常简单，随时调用随时使用。

先引入文件：
````
<script type="text/javascript" src="./src/js/waterfall.js"></script>
````

然后在`$(document).ready(function (){})`中使用下列示例。
````
var w = new waterfall(); //实例化
w.$target = $('#panel'); //设定外围容器
w.$items = '.item'; //设定瀑布流元素的jquery string
w.marginLeft = 10; //间隔
w.marginRight = 10;
w.marginTop = 10;
w.marginBottom = 10;
w.init(); //计算和生成瀑布流
````
注意，调用init时必须保证所有的瀑布流元素的DOM已经存在并且可见。

# License

MIT

