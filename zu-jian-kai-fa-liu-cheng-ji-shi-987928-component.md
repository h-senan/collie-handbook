# \# collie项目开发手册

# \#\# 常用vscode插件

# 

# 插件名 \| 功能

# :-\|:-

# change-case\| 变量名格式转换\(驼峰转肉串\)

# Path Intellisense\|路径字符串自动补全

# Project Manager\|多项目一键切换

# TODO Highlight\|高亮'TODO'

# Vetur\|vue格式文件代码高亮

# Auto Rename Tag\|html标签自动书写

# 

# \#\# 组件\(component\)开发要点

# 

# \#\#\# css 命名

# 采用以“组件名”开头的短横杆式+驼峰+下划线混合命名法（aaa-abcDE\_abc）

# 以carousel轮播组件为例：

# \`\`\`html

# &lt;style lang="sass" scoped&gt;

# .carousel-container

#   position: relative

#   

# .carousel-img

#   width: 100%

#   height: 100%

# 

# &lt;/style&gt;

# \`\`\`

# \#\#\# js

# \#\#\#\# props 传值

# 采用以“组件名”开头的驼峰命名法（aaaBc\)

# 例：

# \`\`\`javascript

# props = {

#     carouselDots: Boolean,         //是否显示面板指示点

#     carouselAutoplay: Boolean,     //是否自动切换

#     carouselInterval: String,      //自动切换时间间隔

#     carouselDuration: String,      //滑动动画时长

#     carouselImgUrl: Array,         //轮播图片地址

#     carouselLinks: Array,          //图片跳转地址

#   };

# \`\`\`

# \#\#\#\# pages-data传入组件数据

# 采用以“组件名”开头+数字+驼峰命名法（aaa1Bc）同一页面中多次调用相同组件传入组件data以数字区分

# 例：

# \`\`\`javascript

# data = {

#     carouselDots: true,

#     carouselAutoplay: true,

#     carouselInterval: '2000',

#     carouselDuration: '500',

#     carouselImgUrl: \[

#       "http://img02.tooopen.com/images/20150928/tooopen\_sy\_143912755726.jpg",

#       "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175866434296.jpg",

#       "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175833047715.jpg"

#     \],

#     carousellinks: \["url1", "url2", "url3"\],

# 

#     carousel2Dots: true,

#     carousel2Autoplay: true,

#     carousel2Interval: '1000',

#     carousel2Duration: '800',

#     carousel2ImgUrl: \[

#       "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175866434296.jpg",

#       "http://img02.tooopen.com/images/20150928/tooopen\_sy\_143912755726.jpg",

#       "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175833047715.jpg"

#     \],

#     carousel2links: \["url1", "url2", "url3"\]

#   };

# \`\`\`

# 

# 

# 

# 

# 

# 

# 



