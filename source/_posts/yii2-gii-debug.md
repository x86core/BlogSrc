---
title: yii2 gii & debug
date: 2017-10-11 17:55:07
tags: Yii2
---
>> 开发环境下的gii和debug使用

### 虚拟机 403 问题
默认只允许本地访问，需要配置allowedIPs允许访问的IP。

``` php 
    $config['bootstrap'][] = 'debug';
    $config['modules']['debug'] = [
        'class' => 'yii\debug\Module',
        'allowedIPs' => ['127.0.0.1', '::1', '192.168.*.*']
    ];

    $config['bootstrap'][] = 'gii';
    $config['modules']['gii'] = [
        'class' => 'yii\gii\Module',
        'allowedIPs' => ['127.0.0.1', '::1', '192.168.*.*']
    ];
```
