# D3.js Learning

> [D3](http://d3js.org)是一个JavaScript库，用于创建数据可视化图形。D3是一个缩写，它的全称叫Data-Driven Documents(数据驱动的文档)。数据来源于你，而文档就是基于 Web的文档(或者网页)，代表可以在浏览器中展现的一切，比如 HTML、SVG。D3扮演的是一个驱动程序的角色，因为它联系着数据和文档。

不同于探索型工具如[Tableau](http://www.tableausoftware.com)和[ggplot2](http://ggplot2.org)，D3擅长生成解释型视图，不擅长探索型视图。


### 可视化工具汇总
**1.简易图表**
* [DataWrapper](http://datawrapper.de)

一个非常漂亮的在线服务，上传数据并快速生成图表后，就可以到处使用或将其嵌入在自己的站点中。这个服务最初定位于专栏记者，而实际上任何人都可以使用。DataWrapper在新版本浏览器中可以显示动态图表，而在旧版本浏览器中则显示静态图片。你也可以下载代码在自己的服务器上运行。

* [Flot](http://www.flotcharts.org)

一个基于jQuery的绘图库，使用HTML的canvas元素，也支持旧版本浏览器(甚至 IE6)。它支持有限的视觉形式(折线、散点、条形、面积)，但使用很简单。

* [Google Chart Tools](https://developers.google.com/chart/)

由早期的Image Charts API发展而来的Google Chart Tools，可以用来生成不少标准的图表，也支持旧版本的IE。

* [gRaphaël](http://g.raphaeljs.com)

基于Raphaël(参见本节后面)的一个图表库，支持旧版本浏览器(包括 IE6)。与 Flot相比，它更灵活，而且据说还要更漂亮一些。

* [Highcharts JS](http://www.highcharts.com)

JavaScript图表库，包含一些预定义的主题和图表。它在最新浏览器中使用SVG，而在旧版本IE(包括IE6及更新版本)中使用后备的 VML。这个工具只对非商业用途免费。

* [JavaScript InfoVis Toolkit](http://philogb.github.com/jit)

简称JIT，它提供了一些预设的样式可用于展示不同的数据，包括很多例子，而文档的技术味道太浓。如果你喜欢它的预设样式，可以选择它，但浏览器支持情况不太清楚。

* [jqPlot](http://www.jqplot.com)

jQuery绘图插件，只支持一些简单的图表，适合不需要自定义样式的情况。jqPlot支持IE7及更新版本。

* jQuery Sparklines

可生成波形图的jQuery插件，主要是那些可以嵌在字里行间的小条形图、折线图、面积图。支持大多数浏览器，包括IE6。

* [Peity](http://benpickles.github.com/peity/)

jQuery插件，可生成非常小的条形图、折线图和饼图，只支持较新版本的浏览器。再强调一遍，它能生成非常小又非常精致的小型可视化图表，可爱程度加10分。

* [Timeline.js](http://timeline.verite.co/)

专门用于生成交互式时间线的一个库。不用编写代码，只用其代码生成器即可。定制的空间不大，但时间线可不是那么容易做的。Timeline.js只支持IE8及之后的版本。

* [YUI Charts](http://yuilibrary.com/yui/docs/charts/)

雅虎YUI(Yahoo! User Interface Library)的Charts模块，可用于创建简单的图表，支持很多浏览器。

**2.图谱可视化**
>  所谓“图谱”，就是具有网络结构的数据(比如 B 连接到 A，A 连接到 C)。

* [Arbor.js](http://arborjs.org/)

基于jQuery的图谱可视化库。就算没用过它，也该看一看它的文档，连它的文档都是用这个工具生成的(可见它有多纯粹、多meta)。这个库使用了HTML的canvas元素，因此只支持IE9和其他较新的浏览器，当然也有一些针对旧版浏览器的后备措施。

* [Sigma.js](http://sigmajs.org/)

一个非常轻量级的图谱可视化库。无论如何，你得看看它的网站，在页面上方的大图上晃几下鼠标，然后再看看它的演示。Sigma.js很漂亮，速度也快，同样使用canvas。

**3.地图映射**
> 我们要区分一下地图(全部内容都是地图)和地图映射(包括地理位置数据或地理 数据，比如传统的地图)。D3 本身也有很多地图映射功能，但下面这些工具最好你 也了解一下。

* [Kartograph](http://kartograph.org)

Gregor Aisch开发的一个基于JavaScript和Python的非常炫的、完全使用矢量的库，它的演示是必看的。最好现在就去看一看。保证你从来没见过这么漂亮的在线地图。Kartograph支持IE7及更新版本。

* [Leaflet](http://leafletjs.com)

贴片地图的库，可以在桌面和移动设备上流畅地交互。它支持在地图贴片上显 示一些SVG数据层。(参见Mike的演示“Using D3 with Leaflet”:http://bost. ocks.org/mike/leaflet/。) Leaflet支持IE6(勉强)或IE7(好得多)，当然还有其他更新版本的浏览器。

* [Modest Maps](http://modestmaps.com/)

作为贴片地图库中的老爷爷，Modest Maps已经被Polymaps取代了，但很多人还是喜欢它，因为它体积小巧，又支持IE和其他浏览器的老版本。Modest Maps有很多版本，包括ActionScript、Processing、Python、PHP、Cinder、openFrameworks...... 总之，它属于老当益壮那种。

* [Polymaps](http://polymaps.org/)

显示贴片地图的库，在贴片上可以叠加数据层。Polymaps依赖于 SVG，因此在较新的浏览器中表现很好。

**4.较原始的方案**
> 以下工具跟 D3 有些类似，都提供了绘制图形的方法，但没有预定义的模板。如果你愿意从头开始，希望得到更大的自由度，可能会对它们感兴趣。

* [Processing.js](http://processingjs.org/)

Processing的原生JavaScript实现，是新接触编程的艺术家和设计师的梦幻式编程语言。Processing是Java写的，因此 Processing草图要在网页中显示通常要靠Java小程序。有了 Processing.js，常规的Processing代码就可以在浏览器中直接运行了。由于使用canvas，所以只适合现代的浏览器。

* [Paper.js](http://paperjs.org/)

在canavs上渲染矢量图形的框架。同样，它的网站也堪称互联网上最
漂亮的网站之一，它们的演示做得让人难以置信。

* [Raphaël](http://raphaeljs.com)

也是一个绘制矢量图形的库，受欢迎的原因是语法具有亲和力，而且支持老版本 浏览器。

**5.三维图形**
> 说来也怪，D3不擅长3D，因为浏览器从一开始就是二维的东西。但随着它对WebGL的支持越来越完善，在网页中显示3D图形也会渐渐成为一种趋势。

* [PhiloGL](http://www.senchalabs.org/philogl/)

专注于3D可视化的一个WebGL框架。

* [Three.js](http://mrdoob.github.com/three.js/)

能帮你生成任何3D场景的一个库，谷歌Data Arts团队出品。它的演示可以让人整整一天都沉浸其中，兴奋不已。

**6.基于D3的工具**
> 如果你使用 D3，但又不想写代码，可以考虑下面这些基于D3的工具。

* [Crossfilter](http://square.github.com/crossfilter/)

一个可以操作大型、多元数据集的库，主要作者是Mike Bostock。非常适合把你的“大数据”塞到相对小的浏览器里。

* [Cubism](http://square.github.com/cubism/)

时间序列数据可视化的D3插件，也是Mike Bostock写的。(我非常喜欢其中的 演示。

* [Dashku](https://dashku.com/)

用于实时更新在线控制板和小部件的在线工具，作者是Paul Jensen。

* [dc.js](http://nickqizhu.github.com/dc.js/)

这里的“dc”是dimensional charting(维度图表)的简写，因为这个库是专门为探索大型、多维数据集而进行优化的。

* [NVD3](http://nvd3.org/)

可重用的D3图表。NVD3提供了很多漂亮的示例，不用像在D3里那样编写代码就可以定制很多效果。

* [Polychart.js](http://code.shutterstock.com/rickshaw/)

更多可重用的图表，可选择的图表类型非常之多。Polychart.js 只对非商业用途免费。

* [Rickshaw](http://code.shutterstock.com/rickshaw/) 

显示时间序列数据的一个工具包，提供了很多定制选项。

* [Tributary](http://tributary.io/)

实时测试D3代码的一个好工具，作者是Ian Johnson。

