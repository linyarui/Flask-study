# Flask-study
一、flask的特点

1、微框架、简洁、只做需要做的，给开发者提供很大的扩展性。

2、Flask和相关的依赖（Jinja2、Werkzeug）设计得非常优秀，用起来很舒服。

3、开发效率非常高，比如使用SQLAlchemy的ORM操作数据库可以节省开发者大量书写sql的时间。

4、使用Flask开发数据库的时候，具体是使用SQLAlchemy还是MongoEngine或是不用ORM而直接基于MySQL-Python这样的底层驱动进行开发都是可以的，选择权完全掌握在你自己手中。区别于Django，Django内置了非常完善和丰富的功能，并且如果你想替换成你自己想要的，要么不支持，要么非常麻烦。

5、Flask把默认的Jinja2模板引擎替换成Mako引擎或者其他模板引擎都是非常容易的。


二、第一个Flask程序

# coding: utf8

# 从flask框架中导入Flask类
from flask import Flask

# 传入__name__初始化一个Flask实例
app = Flask(__name__)


# app.route装饰器映射URL和执行的函数。这个设置将根URL映射到了hello_world函数上
@app.route('/')
def hello_world():
    return 'Hello World!'


if __name__ == '__main__':
    # 运行本项目，host=0.0.0.0可以让其他电脑也能访问到该网站，port指定访问的端口。默认的host是127.0.0.1，port为5000
    app.run(host='0.0.0.0', port=9000)
