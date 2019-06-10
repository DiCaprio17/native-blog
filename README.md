# fruits-and-vegetables
基于python3.6

根据廖雪峰的Python教程改写的原生Python实现网上个人博客，包含日志、用户和评论部分
# 主要功能
- 用户的注册，登陆，注销
- 发布新日志，编辑存在日志
- 用户发布日志评论
- 管理日志，用户及日志评论
# 搭建开发环境
`$ pip3 install aiohttp jinja2 aiomysql markdown`
# 配置
## 数据库
执行`conf/create_tables.sql`创建表
## mysql

    configs = {
	    'debug': True,
	    'db': {
	    'host': '127.0.0.1',
	    'port': 3306,
	    'user': 'root',
	    'password': '123456',
	    'db': 'awesome'  # 数据库名称
	    },
	    'session': {
	    'secret': 'Awesome'
	    }
    }

# 启动
`python3 app.py`