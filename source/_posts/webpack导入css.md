---
title: webpack导入css
date: 2017-11-13 17:31:58
tags:
---

#### webpack 导入css模块

- 安装loader
    npm install style-loader css-loader postcss-loader
  说明： postcss-loader 添加浏览器前缀。

- webpack 配置
    conf/webpack.base.conf.js 文件

``` js
module:{
    rules:[
        ...
        {
            test:/\.css$/,
            loader:'style-loader!css-loader!postcss-loader',
            include: []   //不可省，否则可能导致无法加载模块，原因：未知
        }
        ...
    ]
}
```


- 使用main.js
``` js
import '<dir>/demo.css'
```