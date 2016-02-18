# fsBanner
fsBanner手风琴特效jquery插件
其中该特效需要引入jquery 和 fsbanner.js以及fsbanner.css文件。

在页面上的DOM元素加载完毕之后，可以通过fsBanner()的方法来初始化该插件。
语法结构为：
    $('.fsbanner').fsbanner(options);
    
    且它的配置参数为：
        
  参数	      值	               默认值	          描述
showName	true / false	          true	    如果设置为true， .name 元素将被显示在Banner的左下方
trigger	  click / mouse	          click	    使用哪种方式来触发手风琴的展开和收缩
toUpdate	    hash	                {}	    当你展开一个Banner的时候，脚本会从它的HTML元素中的span元素中获取信息。你可以通过这个选项来使用这些值去更新其它元素。
whenEmpty	    hash	                {}	    当没有Banner展开的时候（初始化时或重置banner宽度的时候），就不会有消息显示在toUpdate选项中指定的元素中。
hideParent	selector	            null	    如果设置了该选项，whenEmpty参数将被忽略。当没有banner同时又设置了hideParent的时候，脚本将隐藏传入的选择器元素。
onChanged	  function	            null	    当banner被展开的时候该函数将被触发。它接收2个参数：展开的banner和之前展开的banner。这些参数是jQuery选择器。
