

启动 zipkin server
```shell
$ docker run -d -e RABBIT_ADDRESSES=192.168.163.41:5672 -e RABBIT_USER=admin -e RABBIT_PASSWORD=123456 -e RABBIT_VIRTUAL_HOST=/dev -e RABBIT_QUEUE=zipkin -p 9411:9411 openzipkin/zipkin
```

浏览器访问

<http://192.168.163.41:9411/zipkin/>

再启动微服务查看效果