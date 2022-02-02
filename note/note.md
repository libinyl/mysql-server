# 存储引擎要实现哪些接口?

```
Each storage engine is a class with each instance of the class communicating with the MySQL server through a special handler interface.
```

- 每个存储引擎都是一个类. 这个类的每个实例都通过一个特殊的`handler`接口与mysql server通信.
- 每个链接对应一个存储引擎实例.如果有三个访问一个表,那就需要创建三个实例. 

- 参考官方指引: https://dev.mysql.com/doc/internals/en/custom-engine.html