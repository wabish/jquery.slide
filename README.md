# jquery.slide

> A simple jQuery slider.

## Installing with NPM

``` bash
$ npm install jquery.slide --save
```

## Installing with Bower

``` bash
$ bower install jquery.slide --save
```

## Demo
[https://cobish.github.io/jquery.slide/](https://cobish.github.io/jquery.slide/)

## How to use

First include the ``jquery.slide.css`` file, you can also create your own style file.

``` css
<link rel="stylesheet" href="./css/jquery.slide.css" />
```

Simply include the `jquery.slide.min.js` file and place the following in the head of your document (make sure **jQuery** is included).

``` js
<script src="../dist/lib/jquery-1.11.1.min.js"></script>
<script src="../dist/jquery.slide.min.js"></script>
```

### Minimum setup

``` javascript
$(function() {
  $('.slide').slide();
});
```

#### Example with default options

``` javascript
$(function() {
  $('.slide').slide({
    isAutoSlide: true,                // 自动轮播
    isHoverStop: true,                // 鼠标移上是否停止轮播
    isBlurStop: true,                 // Window失去焦点是否停止轮播
    isShowDots: true,                 // 是否显示状态点
    isShowArrow: true,                // 是否显示左右箭头
    isHoverShowArrow: true,           // 是否鼠标移上才显示箭头
    isLoadAllImgs: false,             // 是否一次性加载完全部图片
    slideSpeed: 10000,                // 轮播速度 (ms)
    switchSpeed: 500,                 // 图片切换速度 (ms)
    dotsClass: 'dots',                // 状态点样式
    dotActiveClass: 'active',         // 状态点激活样式
    dotsEvent: 'click',               // 状态点事件，click或mouseover或mouseenter
    arrowClass: 'arrow',              // 箭头样式
    arrowLeftClass: 'arrow-left',     // 左箭头样式
    arrowRightClass: 'arrow-right'    // 右箭头样式
  });
});
```

## License

This plugin is available under [the MIT license](http://mths.be/mit).
