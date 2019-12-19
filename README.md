# 安装python3.6和pip3
# 安装依赖
pip3 install -r requirements.txt
# 启动服务
python3 main.py
# 域名解析配置
打开域名管理，以阿里云为例，加入两条信息

加入一条A记录，指向我们将要部署的服务IP地址
```
A	mx	 103.216.2xx.1xx
```

加入一条MX记录，指向上面配置的收邮件的域名地址。
```
MX	*	mx.miniprogram.work
```

> 然后所有发送给xxxx@mx.miniprogram.work的邮件都会被收到了
# 参考
https://s0aiosmtpd0readthedocs0io.icopy.site/en/latest/

