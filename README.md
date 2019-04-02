#安装python3和pip3
#安装依赖
pip3 install -r requirements.txt
#启动服务
python3 main.py
# 域名解析配置
打开域名管理，以阿里云为例，加入两条信息

加入一条A记录，指向我们将要部署的服务IP地址
```
A	mx	 103.216.2xx.1xx
```

加入一条MX记录，指向上面配置的收邮件的域名地址。
```
MX	*	mx.tanyuelab.top
```

> 然后所有发送给xxxx@mx.tanyuelab.top的邮件都会被收到了


