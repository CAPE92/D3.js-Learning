# D3.js Learning

> [D3](http://d3js.org)是一个JavaScript库，用于创建数据可视化图形。D3是一个缩写，它的全称叫Data-Driven Documents(数据驱动的文档)。数据来源于你，而文档就是基于 Web的文档(或者网页)，代表可以在浏览器中展现的一切，比如 HTML、SVG。D3扮演的是一个驱动程序的角色，因为它联系着数据和文档。

不同于探索型工具如[Tableau](http://www.tableausoftware.com)和[ggplot2](http://ggplot2.org)，D3擅长生成解释型视图，不擅长探索型视图。


可视化工具汇总
简易图表
* DataWrapper
一个非常漂亮的在线服务，上传数据并快速生成图表后，就可以到处使用或将其 嵌入在自己的站点中。这个服务最初定位于专栏记者，而实际上任何人都可以使 用。DataWrapper 在新版本浏览器中可以显示动态图表，而在旧版本浏览器中则显示静态图片。(太聪明了!)你也可以下载代码在自己的服务器上运行。地址: http://datawrapper.de/。
* Flot
一个基于 jQuery 的绘图库，使用 HTML 的 canvas 元素，也支持旧版本浏览器
(甚至 IE6)。它支持有限的视觉形式(折线、散点、条形、面积)，但使用很简 单。地址:http://www.flotcharts.org/。
• Google Chart Tools
由早期的Image Charts API发展而来的Google Chart Tools，可以用来生成不少 标准的图表，也支持旧版本的 IE。地址:https://developers.google.com/chart/。
• gRaphaël
基于 Raphaël(参见本节后面)的一个图表库，支持旧版本浏览器(包括 IE6)。与 Flot 相比，它更灵活，而且据说还要更漂亮一些。地址:http://g.raphaeljs.com/。
• Highcharts JS
JavaScript 图表库，包含一些预定义的主题和图表。它在最新浏览器中使用 SVG， 而在旧版本 IE(包括 IE6 及更新版本)中使用后备的 VML。这个工具只对非商 业用途免费。地址:http://www.highcharts.com/。
• JavaScript InfoVis Toolkit
简称 JIT，它提供了一些预设的样式可用于展示不同的数据，包括很多例子，而 文档的技术味道太浓。如果你喜欢它的预设样式，可以选择它，但浏览器支持情 况不太清楚。地址:http://philogb.github.com/jit/。
• jqPlot
jQuery 绘图插件，只支持一些简单的图表，适合不需要自定义样式的情况。jqPlot 支持 IE7 及更新版本。地址:http://www.jqplot.com/。
• jQuery Sparklines
可生成波形图的 jQuery 插件，主要是那些可以嵌在字里行间的小条形图、折线 图、面积图。支持大多数浏览器，包括 IE6。地址:http://omnipotent.net/jquery. sparkline/#s-about。
• Peity
jQuery 插件，可生成非常小的条形图、折线图和饼图，只支持较新版本的浏览 器。再强调一遍，它能生成非常小又非常精致的小型可视化图表，可爱程度加 10 分。地址:http://benpickles.github.com/peity/。
• Timeline.js
专门用于生成交互式时间线的一个库。不用编写代码，只用其代码生成器即可。 定制的空间不大，但时间线可不是那么容易做的。Timeline.js 只支持 IE8 及之后 的版本。地址:http://timeline.verite.co/。
• YUI Charts
雅虎YUI(Yahoo! User Interface Library)的Charts模块，可用于创建简单的图 表，支持很多浏览器。地址:http://yuilibrary.com/yui/docs/charts/。


