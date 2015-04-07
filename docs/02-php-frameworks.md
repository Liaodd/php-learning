# PHP框架，以及我最熟悉的框架

下面是我自己的话：

```
为什么要使用框架进行开发？
1. 框架提供了一个集中的方式来管理请求（request、routing）与输出。
2. 一般的框架都是MVC架构，代码更加清晰。
3. 提供了一系列的工具类来方便开发，提升开发效率。
4. 配合web容器（apache或者nginx）的url rewrite，提供了更美观的url，提升SEO（也许未来的搜索引擎已经不在乎url如何）

正如上面提到的好处，框架也会带来一些劣势，最重要的一点就是性能消耗，不过现在的服务器性能好，为了这些好处放弃一些性能也不是什么问题
```
## PHP框架 yaf

```
https://github.com/laruence/php-yaf
Watch 280 Star 1478 Fork 639 // 数据截止至：2015-04-07 14:15:39
```

绝大部分的PHP框架都是PHP写的，在执行过程当中总会出现解释的过程，这是很多人反对框架的其中一个理由。

于是国内的著名PHP大牛[鸟哥惠新宸](http://weibo.com/laruence)用C开发了一个PHP框架——[yaf](https://github.com/laruence/php-yaf)

```
PHP framework written in c and built as a PHP extension.
```

这个框架的性能极好，因为C性能本来就好……

有这个框架的存在，我觉得部分C/C++开发者在接触PHP的过程当中，说不定也可以用C/C++来实现部分功能，安装成一个PHP扩展，比如一些私有协议的RPC调用功能。

## PHP框架 CodeIgniter

```
https://github.com/bcit-ci/CodeIgniter/
Watch 1366 Star 9652 Fork 4964 // 数据截止至：2015-04-07 14:18:11
```

## PHP框架 Yii

```
https://github.com/yiisoft/yii
Watch 553 Star 4342 Fork 1848 // 数据截止至：2015-04-07 14:23:14
```

## PHP框架 Laravel

```
https://github.com/laravel/laravel
Watch 2192 Star 15643 Fork 5018 // 数据截止至：2015-04-07 14:23:19
```

## PHP框架 kohana

```
https://github.com/kohana/kohana
Watch 147 Star 1437 Fork 375 // 数据截止至：2015-04-07 14:25:39
```

## 我最熟悉的框架 kohana

我最熟悉的框架是Kohana，这个框架是上述5个里面最不火的，为什么会选择它呢，因为我就只熟悉这个框架……拿熟悉的来进行开发成本最最低了。

没记错的话，kohana的诞生是因为一群开发者不满CI（CodeIgniter）框架更新缓慢，而搞出的一个新框架。其1.0版本跟CI差不多，2.0版本已经大幅改变，不过还能看到一点点CI的影子，而3.0版本已经改头换面了。

通过这个框架源码的阅读，我发现了git上的一个很有用的东西，就是`git submodule`，看看kohana的源码，能发现他是各种子项目合成的一个大项目。

在这个框架的[官网](https://kohanaframework.org/)上有自己的详细介绍，为什么要选择它。

这个框架我最喜欢的是其中的[Cascading Filesystem](https://kohanaframework.org/3.3/guide/kohana/files)系统，详情可以点击链接查看，下面从官网盗图过来：

![Kohana Framework Cascading Filesystem](https://kohanaframework.org/3.3/guide-media/kohana/cascading_filesystem.png)

简单的说，系统会自动从上到下的合并你的所用同名的目录和覆盖同名的文件，提升灵活性。

## 最后的一些话

我觉得，选择框架的过程中，如果有开发者对某个框架最熟悉，就可以选择他，如果都不熟，就选个最火的。
