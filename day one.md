#  一灯学堂14天训练营笔记(第一天)

## crossorigin属性

> 在HTML5中，一些 HTML 元素提供了对 [CORS](https://developer.mozilla.org/en-US/docs/HTTP/Access_control_CORS) 的支持， 例如 `img`和`script`均有一个跨域属性 (`crossOrigin` property)，它允许你配置元素获取数据的 CORS 请求。 这些属性是枚举的，并具有以下可能的值：

* anonymous: 对此元素的CORS请求将不设置凭据标志。
* use-credentials: 对此元素的CORS请求将设置凭证标志; 这意味着请求将提供凭据。

## 图片计算网速的技巧

原理： 利用JS去加载一张图片，然后计算出时间差，再利用图片的大小(kb)除以时间得到 kb/s，也就是网速，下面是示意代码：

```js
var s = Date.now();
var image = new Image();
image.crossOrigin = 'anonymous'; // 允许跨域
image.src = 'http://xxx.png';
img.onload = funciton () { // 图片加载完毕的回调函数
  var e = Date.now();
  var netSpeed  = 4 / (e - s) // 假设这里是4kb的图片
}
```

## 图片可以用来埋点

原理：避免Ajax的性能浪费，巧用image的访问记录来做埋点，

PS: Ajax是非常珍贵的, 很多网站的Ajax并发是5个

## CSS远程攻击漏洞

background的url是可以执行js的(有些浏览器)

## 渲染

尽量减少dom的数量，多使用如伪类伪元素，因为CSS是GPU渲染的，所以性能比dom tree的渲染好很多。

PS: 一个简单的dom有太多太多的东西了，可以for in 遍历查看一个dom的属性

## JSONP
原理：借助Script标签来加载远程的JS函数

## document.domain和iframe通信的技术细节

## 跨域：协议，端口，域名不一样就是不同的域名

## HTML5语义化

> 根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的同时让浏览器的爬虫和机器很好地解析。










