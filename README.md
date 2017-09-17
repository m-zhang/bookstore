# bookstore

采用Mocha(测试框架)、chai（断言库像should、expect这些） 测试Node RESTful API，之前项目多用postman来做些简单的测试.感谢Samuele Zaza的这篇教程：[Test a Node RESTful API with Mocha and Chai](https://scotch.io/tutorials/test-a-node-restful-api-with-mocha-and-chai) 

如果对英文阅读有困难的童鞋可以参考阮一峰老师的[测试框架 Mocha 实例教程](http://www.ruanyifeng.com/blog/2015/12/a-mocha-tutorial-of-examples.html) 简单比较容易理解。

说明：将项目代码clone 到本地，安装pakeage.json里面的相关文件依赖。
```javascript
//运行测试用例 mocha --timeout 10000
npm test

```

项目源码中有两点需要注意安装mocha后会自动检索项目根目录下test路径，运行测试用例js文件，还有一点就是利用require('config')来加载/config 路径下的配置文件默认default.json,在运行测试用例需通过设置process.env.NODE_ENV = 'test'来切换到测试数据库。
