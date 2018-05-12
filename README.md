# AKjs.Mobile v 1.1.0
AKjs前端框架是Andrew.Kim和他的团队一起研发的基于jQuery的一个轻量级前端框架。它是只要懂jQuery的语法很容易上手的框架。该框架里面现在发布了很多移动端常用的功能效果；开发者们使用过程中功能插件也可以自己扩展增加。另一方面，它是相当于一个丰富的组件化UI框架，优点是开发要前后端分离，项目开发过程中后端通过ajax调用数据的机制。

AKjs是一个基于jQuery的一套构建用户界面的前端框架，插件里包含着移动端常用的功能效果以及简单明了的CSS样式库，对IOS和安卓系统的兼容性很完美。支持前后端分离开发和路由模式跳页方式。它与其他重量级框架不同的是AKjs采用了按需引入插件功能以及所有的UI布局中可以让用户自行发挥写页面，因为它提供的CSS库模块化的很细分，让开发者们可以轻松的解决前端的烦恼。

注：开发正式项目的时候不要用demo.html里的内容，该文件只是静态演示版用的文件。为了更好的体验效果开发项目的时候请使用index.html。


预览效果 http://118.244.206.115:8080/ak/

AKjs前端技术支持QQ群：724501394

# 更新时间：2018/5/09 下午 16:36

# 更新说明：

js目录和css目中 akjs.mobile.js 和 akjs.mobile.css 发布 1.1.0版本；

修改不走路由功能时界面加载失败的bug以及聊天界面的输入框焦点时头部区域漂浮的问题。

增加以下几个功能

Andrew_setCookie & Andrew_getCookie & Andrew_delCookie 使用方法：

Andrew_setCookie("username", user, 365); //设置cookie

var user = Andrew_getCookie("username"); //获取cookie

Andrew_delCookie(name) //删除cookie

Andrew_htmlEncode & Andrew_htmlDecode 使用方法：

Andrew_htmlEncode(str); //把TEXT转换HTML

Andrew_htmlDecode(str); //把HTML转换TEXT


# 更新时间：2018/5/08 下午 16:30

# 更新说明：

js目录和css目中 akjs.mobile.js 和 akjs.mobile.css 发布 1.0.9版本；

解决页面刷新时布局有变形的bug以及Andrew_Unicode的函数，把中文转换Unicode。

增加以及修改几个功能插件：

增加 js/plugin/Andrew_QRcode.js //二维码生成插件

增加 js/plugin/Andrew_Marquee.js //上下左右滚动插件

增加 js/plugin/Andrew_TypeIt.js //文字打字效果插件

增加 js/plugin/Andrew_Vticker.js //列表垂直滚动插件

修改 js/plugin/Andrew_Tabs.js //修改tabs功能中的回调函数

修改 js/plugin/Andrew_Select.js //解决界面先后加载顺序问题

修改 js/plugin/Andrew_Form.js //解决界面先后加载顺序问题

修改 js/plugin/Andrew_DropLoad.js //解决有些设备下拉滑动时卡顿的问题

修改 js/plugin/Andrew_NavScroll.js //导航滑动时增加弹性效果

最后请把js目录中的plugin.js文件进行替换。


# 更新时间：2018/5/02 下午 14:35

# 更新说明：

js目录和css目中 akjs.mobile.js 和 akjs.mobile.css 发布 1.0.8版本；

解决通过安卓端微信浏览器访问时页面白屏的bug；

演示版的引导页增加动画效果；请替换router/start.html 即可。

修改js/plugin/Andrew_Slider.js功能插件，增加循环设置参数（loopPlay）。


# 更新时间：2018/4/26 下午 13:20

# 更新说明：

js目录和css目中 akjs.mobile.js 和 akjs.mobile.css 发布 1.0.7版本；

--这次升级是主要解决混合开发APP的时候IOS版本不兼容window.location.href方法跳页的问题，所以这次版本中封装了 Andrew_Location 功能解决兼容问题。

--还有为了后台开发方便封装了Andrew_getUrlParam 获取URL中的参数值的方法和Andrew_changeURLArg更改URL中的参数值的方法。

以上三个功能的使用方法在打开router.js文件中的第63行代码部分即可。

1.0.7版本中增加了Andrew_Include功能；是js文件中引入另一个js文件的功能。也可以在js文件中引入css样式。

Andrew_Include使用方法(在js代码中使用)： 

js引入 - Andrew_Include("file.js","js"); 或者 Andrew_Include("file.js");

css引入 - Andrew_Include("file.css","css");

原先data.js文件在router.js文件中通过Andrew_Include的方法引入到演示版项目中。


# 更新时间：2018/4/25 下午13:00

# 更新说明：

增加 js/plugin/Andrew_Circliful.js 圆形统计插件。

打开 js/plugin.js 文件 插入 Andrew_Plugin("Andrew_Circliful"); 即可用。调用方法在page4.html文件中的最底部。


# 更新时间：2018/4/24 下午15:20

# 更新说明：

发布 AKjs1.0.6版本，并且个别的文件名更改。

andrew.mobile.plugin.js 文件名更改为 akjs.mobile.js

andrew.mobile.style.css 文件名更改为 akjs.mobile.css

andrew.animate.css 文件名更改为 akjs.animate.css

andrew.router.js 文件名更改为 router.js

css/style.css 文件需要替换；

akjs.mobile.js 里新增了Andrew_DateFormat的功能函数；

--- 使用方法：Andrew_DateFormat(new Date(),"yyyy-MM-dd HH:mm") //后台开发时方便与日期格式化

这次新版还新增了 js/plugin/Andrew_Template.js 模板引擎功能插件；

--- 使用方法：$("元素").Andrew_Template(list_data); //该插件的使用方法在router/page4.html中展示了效果，可参考该文件。


# 更新时间：2018/4/20 下午17:05

# 更新说明：

css目中 andrew.animate.css 发布 1.0.2版本 （增加60多种动画效果）；

js目录和css目中 andrew.mobile.plugin.js 和 andrew.mobile.style.css 发布 1.0.5版本；

修改data-href=值带参数的时候无法识别被选中的状态bug；

增加animation参数跟数据结合的调用方式（数据请求的时候直接写Andrew_Animation();可以使用data-animation属性）；


# 更新时间：2018/4/19 下午13:00

# 更新说明：

更新css目录中的andrew.animate.css 文件；

js目中 andrew.mobile.plugin.js 发布 1.0.4版本 （增加 animation参数可方便制作动画效果）；

Andrew_Config功能中animation参数开启（例：元素里加 data-animation="{name: 'zoomIn', duration:1, delay: 0}"） 动画库：andrew.animate.css


# 更新时间：2018/4/18 下午12:30

# 更新说明：

演示版增加仿京东产品分类Tabs功能；

修改 Andrew_CountDown和Andrew_Progress功能插件的bug（在js/plugin/目录下找相关文件进行替换即可）；

css目中 andrew.mobile.style.css 发布 1.0.4版本 （增加 class名h_fill 可以把元素高度设定为屏幕高度）；

Andrew_Config功能中MaskStyle的参数可设置到 style8;


# 更新时间：2018/4/17 下午09:18

# 更新说明：

之前发布的版本中js/plugin.js按需引入有问题，所以该js文件需要重新替换；

Andrew_Progress功能插件增加文字动画效果（在js/plugin/文件中的Andrew_Progress.js和以及该目录中的css文件夹也需要一起替换）；


# 更新时间：2018/4/11 下午17:05

# 更新说明：

js目录和css目中 andrew.mobile.plugin.js 和 andrew.mobile.style.css 发布 1.0.3版本；

Andrew_Config 功能插件增加了 Responsive参数（该参数能设置按屏幕尺寸字体大小自适应变化；开启 true, 停用 false）

js/andrew.router.js 文件中找Andrew_Config功能增加Responsive参数即可。


# 更新时间：2018/4/10 下午16:10

# 更新说明：

增加Andrew_NavScroll功能插件；

演示版的布局界面中使用Andrew_NavScroll插件和分享功能的展示；

js目录和css目中 andrew.mobile.plugin.js 和 andrew.mobile.style.css 发布 1.0.2版本；

js/plugin.js中请加上Andrew_NavScroll的功能插件；

css/style.css文件需要替换（new_icon和footer区域样式有修改）；

底部菜单中增加最新消息图标（添加class名 new_icon）；

js/plugin/Andrew_StepOrder.js 需要替换；

引导页切换页面的过程中有闪屏的情况时，请替换jQuery3.2.1的版本；


# 更新时间：2018/4/03 下午16:50

# 更新说明：

解决上传图片功能插件删除图片时插件报错的bug（请替换一下Andrew_PreviewImage.js）

Andrew_PreviewImage的插件调用部分的参数修改成以下的方式；

webToast: "成功删除!", //删除图片后提示的文字

Del_icon:"icon-bt_quxiao_a", //图片删除图标样式


# 更新时间：2018/3/30 下午8:48

# 更新说明：

AK插件优化，改成轻量级插件（功能插件分离后可按需引入）；

增加下拉加载更多功能；

全部替换为iconfont图标库；

修改插件上拉刷新和下拉加载的数据调用时的bug；

修改底部菜单切换时图标不变的bug；

特别声明：使用jQuery的版本必须3.0以上才能效果完美；


# 主要目录和主要文件说明：

demo.html --- 未开启路由模式的DEMO页面

index.html --- 走路由模式的DEMO页面 （可查看页面切换效果）

js/plugin/ --- 功能插件目录，里面的css目录是相关功能插件的样式文件；

js/andrew.router.js --- 路由管理器（该功能切换页面时无刷新跳页的功能）

js/data.js --- Json数据文件

js/plugin.js --- 按需引入功能插件（按需引入功能插件时后面带css的意思是相关插件有对应的css文件）

layout/main.html --- 整个界面的布局；（该文件夹和文件名可以在路由管理器文件中配置）

router/ --- 通过路由访问的html界面，该文件夹也在路由管理器文件中配置（里面的所有html文件中最底部都调用功能插件的方法）

css/iconfont --- 图标库 (AK图标库地址：http://www.iconfont.cn/collections/detail?cid=8740)

css/andrew.mobile.style.css --- 全局公共样式库（初始使用本插件的开发者们尽量都看看里面的class命名）

css/theme.default.css --- 所有颜色相关的样式文件

css/style.css --- 自定义样式文件（引入第三方插件时通过该css文件进行覆盖样式）
