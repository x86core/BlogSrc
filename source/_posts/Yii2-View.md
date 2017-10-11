---
title: Yii2 View
date: 2017-10-11 16:33:03
tags: Yii2
---
>> 视图参数传递问题。

#### Layout 视图参数传递

``` php action
    $data =  array(
        'key'=>'value'
    );

    /**
     * yii2/base/View.php
     * @params $params
     * custom parameters that are shared among view templates
     **/
    Yii::$app->view->params = $data;
```
```php template
    <?= $this->params['key'] ?>
```

#### 模板视图传参

``` php action
    $this->redner('index', $data);
```
``` php template
    <?= $key ?>
```