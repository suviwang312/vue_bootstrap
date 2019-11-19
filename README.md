# first

首先不会使用vue脚手架请参考   
[vue脚手架安装教程](https://blog.csdn.net/weixin_41056807/article/details/90239795)

### 引入jQuery
和正常使用bootstrap一样，在引入bootstrap之前要引入jQuery插件。

输入指令：`npm install jquery --save -dev`

出现以上为jQuery安装成功。

安装jQuery成功之后，点击：build ->webpack.base.conf.js进行配置。

 - 在function resolve (dir){…}函数的上面添加：`const webpack = require('webpack');`
 - 在`resolve: {…}`的上面添加：
 

```
plugins: [
    new webpack.optimize.CommonsChunkPlugin('common.js'),
    new webpack.ProvidePlugin({
      jQuery: "jquery",
      $: "jquery"
    })
  ],
```
- 在main.js中添加：`import $ from 'jquery'`

使用jQuery

```js
$(function () {
/*js代码*/
 })
```

### 引入Bootstrap
引入指令： `npm install bootstrap3 -s`


在main.js中加入：

```
import 'bootstrap3/dist/css/bootstrap.min.css'
import 'bootstrap3/dist/js/bootstrap.min.js'
```