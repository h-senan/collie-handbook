# css命名规则

## 规则
- 结构: 组件名-子组件名_修饰词
  - 组件名: 描述当前**模块**功能
  - 子组件名: 具体每个**元素**在当前模块的名字，注意不要重复
  - 修饰词: 表示**状态**，例如隐藏，激活，上浮等
- 组件名为多单词时, 采用**驼峰规则**
- 修饰词可选

## 例子
```html
<view class="carousel">
  <view class="carousel-bar">
    <view class="carousel-titleLabel" wx:if="true">轮播</view>
    <view class="carousel-titleLabel_active" wx:if="false">轮播</view>
    <view class="carousel-delete">
      <image class="carousel-deleteIcon" src="../images/close.png"></image>
    </view>
  </view>
</view>
```
