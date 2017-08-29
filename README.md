# Make_a_Web_Page
_优达学城编程入门第二个项目，制作一个简单的网页_

## 框架
> 使用了[bootstrap](http://v3.bootcss.com/)框架，想尝试使用此框架熟悉前端响应式开发部分内容

## 记录和反馈
昨天提交了第一个版本之后就通过了审核，通过只能表示达到了项目规定的要求吧，但是如果想做好还是有很多地方需要改进的。Reviewer给出了部分的建议：

* 最好不要 **越级** 使用 `<h*>`标签，即有了`<h1>`之后再考虑使用`<h2>`等等
> 理由：搜索引擎会把文章中出现的`<h1>`到`<h6>`标签来作为文章的结构与主次，从而进行索引，所以我们要谨慎使用。

* 可以使用bootstrap添加一个modals窗口，用户点击图片之后可以弹出一个窗口显示更加详细的图片信息

* 目前网页在移动设备上效果不太好，可以尝试使用媒体查询，在手机屏幕下，只显示歌手图片，点击图片modal出歌手信息。

* 反馈1:使用Bootstrap框架时需要在引入css之前导入jquery库，不然会报错，我在第一次直接使用bootstrap官网CDN时就出现了这个报错信息，所以需要记住一定要在引入CSS之前导入jquery才行。

* 反馈2：在使用text-indent（就是缩进）属性时，发现没有任何反应，我的文字当时是放在span标签中的，在我查询[MDN该属性信息](https://developer.mozilla.org/en-US/docs/Web/CSS/text-indent)时，描述信息为：`The text-indent CSS property specifies the amount of indentation (empty space) that is put before lines of text in a block.` 也就是该属性需要放在block标签之下才可以，当我在文字外面套一层`div`之后，该属性就可以了。
> 总结：遇到问题了不要慌张，多查阅资料，留意细节之处。

## 构想
* 给当前网页加入导航栏部分，如果可以的话，给导航栏添加响应式。
* 加入歌手短视频，点击图片之后可以跳出一段短小的视频

