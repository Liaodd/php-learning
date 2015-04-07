# PHP语言基本介绍

* [PHP官网](http://php.net)

* [PHP 维基百科词条](http://zh.wikipedia.org/zh/PHP)

* [深入PHP](http://www.php-internals.com/)

* [PHP源代码](https://github.com/php/php-src)

从维基百科中可以看到PHP的版本与历史。

## 用我的话来介绍一下PHP

* 语法跟C类似，C/C++开发者上手迅速

* 变量以`$`开头

* 弱类型

* 使用`include`、`require`、`include_once`、`require_conce`来包含文件，可以使用auto_load来自动包含

* 最强大的类型是`array`

上面5条是我临时想的关键点，其中前面两条用于凑数，大致说一下语法情况。下面说一下后面三条：

### 弱类型

PHP是弱类型语言，而开发PHP的C是强类型语言，[深入PHP](http://www.php-internals.com/)上面有资料这个是由一个结构体和一个联合体一起做到的：

```c

typedef struct _zval_struct zval;
...
struct _zval_struct {
    /* Variable information */
    zvalue_value value;     /* value */
    zend_uint refcount__gc;
    zend_uchar type;    /* active type */
    zend_uchar is_ref__gc;
};

```

```c

typedef union _zvalue_value {
    long lval;                  /* long value */
    double dval;                /* double value */
    struct {
        char *val;
        int len;
    } str;
    HashTable *ht;              /* hash table value */
    zend_object_value obj;
} zvalue_value;

```


原文链接：[变量的结构和类型](http://www.php-internals.com/book/?p=chapt03/03-01-00-variables-structure)


### 文件引用包含

简单的说一下，`include`和`require`都是引用一个外部文件，后面带once的方法就是只引用一次，防止重复引用。

大部分情况用哪个都没问题，不过还是有些区别在于：

* 如果文件不存在，include将会返回一个警告，程序可以继续执行；require会发出一个严重错误，并且无法继续执行

* include可以放在逻辑中执行，每次执行到这一句时才将外部文件引入；尔require不能，他在一开始就讲文件引入，使其变成文件的一部分。

部分PHP框架中引入了[autoload](http://php.net/manual/zh/language.oop5.autoload.php)，点击链接可以查看详情，简单的说这个东西就是：

```
如果在运行中出现了未定义的类，将会自动调用autoload来尝试加载这个类的文件。
```

### 最强大的类型`array`

PHP的`array`可以放入任何类型的数据，其本质是一个`hashtable`，在深入PHP内核中有[说明](http://www.php-internals.com/book/?p=chapt03/03-01-01-hashtable)

看前面提到的PHP弱类型中，联合体`zvalue_value`就有HashTable这个类型。
