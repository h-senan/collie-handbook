# collie

## js

### props 传值

Object命名：“组件名”+Option
key命名：“组件名”开头的驼峰命名法（aaaBc\)

例：

```js
props = {
    carouselOption: Object,
  };
```
carouselOption数据结构：
```js
  carouselOption: {
  carouselDots: Boolean,          // 是否显示面板指示点 默认true
  carouselArrows: Boolean,        // 是否显示箭头 默认false
  carouselAutoplay: Boolean,      // 是否自动切换 默认true
  carouselCircular: Boolean,      // 是否采用衔接滑动 默认true
  carouselVertical: Boolean,      // 滑动方向是否为纵向 默认true
  carouselInterval: Number,       // 自动切换时间间隔 ms 默认2000
  carouselDuration: Number,       // 滑动动画时长 ms 默认800
  carouselHeight: String,         // 轮播组件高度，需要带单位，可以为px,rpx,vh等css单位
  carouselActiveDotColor: String, // 当前选中的指示点颜色 
  carouselImg:[{
              image: '',    // 图片地址
              url: ''       // 图片跳转地址
            }]
  }               
```

### 调用组件页
如何调用组件：
```js
<template> 
  <carouselIDa :carouselOption="carouselIDa"></carouselIDa>
</template>
<template> 
  <carouselIDb :carouselOption="carouselIDb"></carouselIDb>
</template>
```
同一页面多次复用该组件，components命名方式："组件名"+ID+随机字母
例:
```js
components = {
    carouselIDa: Carousel,
    carouselIDb: Carousel
  };
```
data: 传入get请求所需的componentId
```js
data = {
    carouselIDa:{
      componentId: 'wnvoenvjdw'
    },
    carouselIDb:{
      componentId: 'gasfdagfeg'
    },
  };
```
### constant常量

```js
/**
 * 缓存常量
 */

const USER_INFO='userInfo'// 用户信息
const SESSION_ID='sessionId'//header中携带

module.exports={
  USER_INFO,
  SESSION_ID,
}
```



