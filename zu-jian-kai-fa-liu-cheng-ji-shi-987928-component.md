# collie

微信小程序组件命名规范

## css

采用以“组件名”开头的短横杆式+驼峰+下划线混合命名法（aaa-abcDE\_abc）

以carousel轮播组件为例：

```css
<style lang="sass" scoped>
.carousel-container
position: relative
.carousel-img
width: 100%
height: 100%
</style>
```

## js

### props 传值

采用以“组件名”开头的驼峰命名法（aaaBc\)

例：

```js
props = {
carouselDots: Boolean,         //是否显示面板指示点

carouselAutoplay: Boolean,     //是否自动切换

carouselInterval: String,      //自动切换时间间隔

carouselDuration: String,      //滑动动画时长

carouselImgUrl: Array,         //轮播图片地址

carouselLinks: Array,          //图片跳转地址
};
```

### pages-data传入组件数据

采用以“组件名”开头+数字+驼峰命名法（aaa1Bc）同一页面中多次调用相同组件传入组件data以数字区分

例：

```js
data = {
carouselDots: true,

carouselAutoplay: true,

carouselInterval: '2000',

carouselDuration: '500',

carouselImgUrl: \[

  "http://img02.tooopen.com/images/20150928/tooopen\_sy\_143912755726.jpg",

  "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175866434296.jpg",

  "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175833047715.jpg"

\],

carousellinks: \["url1", "url2", "url3"\],



carousel2Dots: true,

carousel2Autoplay: true,

carousel2Interval: '1000',

carousel2Duration: '800',

carousel2ImgUrl: \[

  "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175866434296.jpg",

  "http://img02.tooopen.com/images/20150928/tooopen\_sy\_143912755726.jpg",

  "http://img06.tooopen.com/images/20160818/tooopen\_sy\_175833047715.jpg"

\],

carousel2links: \["url1", "url2", "url3"\]
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



