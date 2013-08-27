highcharts-export-demo
======================

highcharts导出图片测试，三套方案 
 

1、js获取svg 采用js拼装form表单，submit。后台服务器采用batik来将svg转换成图片 png、jpg、pdf

2、js 拼装form表单，参数为 options 和 callback。调用运行在服务器的phantomjs进程来执行（phantomjs highcharts-convert.js -infile options.json -outfile chart.png -scale 2.5 -width 300 -constr Chart -callback callback.js）命令

3、使用highcharts提供的java后台导出demo来生成图片

注意：highcharts官网提供的demo是服务器启动时候就启动服务池不断的轮询接收导出请求

方案2和方案3 都是使用phantomjs服务来做图片处理，但是执行的命令行有所不同，有待继续研究

2013年8月27日  翟玉勇


2013年8月27日更新
第二套方案源代码将于数据挖掘项目完成后提交

服务器策略：
http://www.highcharts.com/component/content/article/2-news/52-serverside-generated-charts
highcharts API：
http://api.highcharts.com/highcharts#yAxis.labels.style
highcharts DEMO：
http://www.highcharts.com/demo/waterfall/skies



