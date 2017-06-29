# 使用URL查看指定配置文件内容的方法：http：// {configserver}：{configserver.port} / {name} / {profile}

例如我们要查看sample-cloud-client-test.properties则请求的地址为：http：// localhost：8888 / config / test 返回的信息按优先顺序包括：config-test。属性，application-test.properties和application.properties因为应用程序被框架认为是默认配置文件。
