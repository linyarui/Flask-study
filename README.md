#一、flask的特点

1、微框架、简洁、只做需要做的，给开发者提供很大的扩展性。

2、Flask和相关的依赖（Jinja2、Werkzeug）设计得非常优秀，用起来很舒服。

3、开发效率非常高，比如使用SQLAlchemy的ORM操作数据库可以节省开发者大量书写sql的时间。

4、使用Flask开发数据库的时候，具体是使用SQLAlchemy还是MongoEngine或是不用ORM而直接基于MySQL-Python这样的底层驱动进行开发都是可以的，选择权完全掌握在你自己手中。区别于Django，Django内置了非常完善和丰富的功能，并且如果你想替换成你自己想要的，要么不支持，要么非常麻烦。

5、Flask把默认的Jinja2模板引擎替换成Mako引擎或者其他模板引擎都是非常容易的。


#二、第一个Flask程序

