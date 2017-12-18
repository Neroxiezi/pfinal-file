# pfinal-file

![](https://img.shields.io/apm/l/vim-mode.svg)
[![](https://img.shields.io/badge/Downloads-4k-red.svg)](https://packagist.org/packages/nancheng/pfinal-array)


**Note:** ```PHP``` ```PHPfile``` ```Validator```  ```file```

这是一个PHP操作文件的简单操作类


## 安装

通过 Composer 安装：

    php composer.phar require nancheng/pfinal-file
---

## 使用

```php

require_once './vendor/autoload.php';
use pf\file\build\File;
    
//读取文件
$res = File::read('./text.txt');

//写入文件
$res1 = File::put('./text.txt','aaaaaaaaa');

```

## 例子

```php
<?php

require_once './vendor/autoload.php';
use pf\file\build\File;


//读取文件
$res = File::read('./text.txt');

//写入文件
$res1 = File::put('./text.txt','aaaaaaaaa');

//文件内容追加
$rs =  File::append('./text.txt', '222');

//获取文件名
$rs =  File::getName('./text.txt');

//获取文件后缀
$rs =  File::getExt('./text.txt');

//获取文件路径
$rs =  File::getPath('./text.txt');

$rs =  File::has('./text.txt');

var_dump($res1);
```