# 简单的轮播图插件
    最近移动端项目中需要一个展示用的轮播图，网上的插件比较复杂，有些功能暂时用不到，所以打算自己写一个简单的轮播图插件，顺便学习一下插件的写法。
## 1.首先我们新建一个`html`文件并输入以下代码
```html
    <!DOCTYPE html>
    <html>
        <head>
            <meta charset="UTF-8">
            <title></title>
        </head>
        <body>
        </body>
    </html>
```
## 2.在`body`标签中创建一个类名为`carousel`的`div`
```html
    <div class="carousel">
			
    </div>
```
## 3.先在`head`标签中引入我们的`style.css`样式，然后在`<body>`标签的最后先引入我们的`jQuery`文件，然后再引入我们的`jquery.carousel.js`文件
```html
    <!DOCTYPE html>
    <html>
        <head>
            <meta charset="UTF-8">
            <title></title>
            <link rel="stylesheet" type="text/css" href="style.css"/>
        </head>
        <body>
            <div class="carousel">
                
            </div>
            <script src="jquery-1.12.1.min.js"></script>
            <script src="jquery.carousel.js"></script>
        </body>
    </html>
```
## 4.在最后创建一个`<script>`标签书写`js`代码，首先用jQuery选择器找到类名为`carousel`的`div`，然后调用`carousel()`方法，方法内传入以下参数
```js
    $(".carousel").carousel({
        imgArray:array,
        height:"150px",
        time:2000
    });
```
+ 第一个参数为轮播图每一页的图片数组
+ 第二个参数为轮播图高度
+ 第三个参数为轮播图自动播放间隔时间
## 5.这样我们的轮播图就完成了，现在只有自动轮播的功能，今后会不断完善