# 使用URL查看指定配置文件内容的方法： 
# HTTP具体支持的请求方式如下：
# http://{config_server}:{config_server.port}//{application_name}/{profile}[/{label}]
# http://{config_server}:{config_server.port}//{application_name}-{profile}.yml
# http://{config_server}:{config_server.port}//{label}/{application_name}-{profile}.yml
# http://{config_server}:{config_server.port}//{application_name}-{profile}.properties
# http://{config_server}:{config_server.port}//{label}/{application_name}-{profile}.properties
例如我们要查看 config-dev.properties 则请求的地址为：http://localhost:8888/config/dev 返回的信息按优先顺序包括：config-dev.properties、application-test.properties 和 application.properties 因为 application 被框架认为默认配置文件。
