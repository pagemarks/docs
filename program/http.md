
## HTTP/1.x
- 长连接: connection: keep-alive
- chunked编码传输: 将实体分块并标明长度,直至长度为0表示结束.实体长度未知(动态计算)
- 字节范围请求
- 请求流水线(Pipelining)
- 请求/响应头host: 虚拟服务器,一ip多网站
- 缓存方式新增:e-tag,cache-control

## HTTP VS HTTPS
- 数据加密: TLS,非对称传输对称秘钥
- 身份验证: CA整数
- 防数据篡改: 中间人

## HTTP/2 VS HTTP/1.x
- 基于二进制: 高效,紧凑
- 多路复用
- 优先级
- 并行处理
- 头部压缩,减少开销
- 服务端推送
