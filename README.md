Q
conflux有如下rpc吗：
1. 某个地址总共挖出区块的数量
2. 分页查询挖出区块的详细信息
A
全节点没有这些RPC，未来scan 可能会提供

Q
在本地的开发环境10个测试账户都没有了 只剩下本身的账号 而且0cfx (用 docker 运行的,重启之后没的)
A
新起一个container 然后看下 log 吧。 https://forum.conflux.fun/t/topic/4280（win 10 通过docker 运行 conflux）

Q
可以将 Conflux Node的WS 和 HTTP都配置成同一个端口吗？
jsonrpc_ws_port= 80 
jsonrpc_http_port=80
A
不可以

Q
发送交易，交易额，低于多少，就显示成0了呢？
A
只有等于0会显示为0, 哪怕是1 Drip 也会显示.
