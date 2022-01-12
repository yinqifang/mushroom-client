# aiya-client
## 关于aiya
字母计划系列的首个项目，取哎呀谐音，目标是提供一个C/S结构的本地化工具用于提升办公效率
## 客户端开发语言
Python
### 发送端
1. 文件切分，防止超过单邮件附件限制
2. 文件加密，防止发送时触发文件扫描导致发送变慢
3. 生成文件提取码
4. 邮件发送，主题增加关键字
### 接收端
1. 通过提取码获取对应邮件
2. 附件提取
3. 文件解密
4. 文件合并
### python转exe
~~~
pip install pyinstaller
python -m PyInstaller CutCutCut.spec
~~~
## 参考文档
* [Python连接RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-one-python.html)
* [Asynchronous consumer example](https://github.com/pika/pika/blob/master/examples/asynchronous_consumer_example.py)