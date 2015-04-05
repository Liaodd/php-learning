# 入门，基本的网站开发知识

```html
<html>
    <head>
        <title>sample page<title>
        <link href="http://path/to/your/style/file.css" media="all" rel="stylesheet" />
    </head>
    <body>
        <h1>this is an sample page</h1>
        <script type="text/javascrpt">
            alert('welcome to this page');
        </script>
        <script src="https://path/to/your/script/file.js"></script>
    </body>
</html>
```

上面展示了一个基本的html文档的内容。

## HTML的部三个重要tag

* html

    html 是根节点，说明这个xml文档是一个html文档

* head

    head 顾名思义就是头部，跟其他协议（tcp、http）类似，头部用于声明文档的一些基本信息

* body

    body 是html中的正文，描述了这个页面的结构


 ## 如何工作

 ### 书籍推荐

 * [HTTP权威指南](http://www.ituring.com.cn/book/844)


 ### 请求

命令行   | GET /index.php HTTP/1.0
--------|-----------------
请求首部 | Host: www.domain.com...


 ### 响应

 * [HTTP状态码](http://zh.wikipedia.org/zh/HTTP%E7%8A%B6%E6%80%81%E7%A0%81)

 * 读取资源

 * 执行脚本
