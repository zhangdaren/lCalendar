lCalendar移动端日期时间选择控件
==========
纯原生js的移动端日期插件，不依赖任何库，体积非常小只有10k
##用法
直接在html页面中引入input标签，绑定三种事件可调出不同的样式插件，对应说明为：`editDate(event)` 呼出日期选择、`editTime(event)`呼出时间选择、`editDateTime(event)`呼出日期时间选择，此外提供`data-hl-calendar`控制最小日期和最大日期：
```
...
<input type="text" readonly="" name="input_date" placeholder="请输入日期" onClick="editDate(event);" data-hl-calendar="2000-01-01,2018-01-29" />
...
```
样式文件记得引入到页面中：
```
...
<link rel="stylesheet" href="lCalendar.css">
...
```
不要忘了引入js文件到页面中：
```
...
<script src="lCalendar.js"></script>
...
```
欢迎来我的博客留言讨论：http://www.cnblogs.com/xfhxbb/p/lCalendar.html


...
...
...
...
...
////////////////////////////////////////////////////////////////////////////////////////////////////////////
fork自：https://github.com/xfhxbb/LCalendar


2018-09-17
因为工作，从Mdate.js用到LCalendar.js，现有项目使用rem单位，Mdate修改不成功，换成LCalendar，然而却已经两年没有更新了。
经过大半天努力，终于调好支持rem单位了，目前是根据750设计稿来设定的rem，需要的童鞋，可自行调整使用(修改lCalendar.css)。
lCalendar.js里，新增两个变量：
topH：当列表显示第一个时，列表顶部的top，原值为8，现值为2
lHeight ：列表每行的高度，现为1rem(原值为1em)，不需要调整了，可以直接拿来就用，注意！这里的高度与css里的高度是对应的，如需修改，需同步。

