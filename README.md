Q <br>
conflux有如下rpc吗：
1. 某个地址总共挖出区块的数量
2. 分页查询挖出区块的详细信息

A <br>
全节点没有这些RPC，未来scan 可能会提供
<br>

Q <br>
在本地的开发环境10个测试账户都没有了 只剩下本身的账号 而且0cfx (用 docker 运行的,重启之后没的)

A <br>
新起一个container 然后看下 log 吧。 https://forum.conflux.fun/t/topic/4280（win 10 通过docker 运行 conflux）
<br>

Q <br>
可以将 Conflux Node的WS 和 HTTP都配置成同一个端口吗？
jsonrpc_ws_port= 80 
jsonrpc_http_port=80

A <br>
不可以
<br>

Q <br>
发送交易，交易额，低于多少，就显示成0了呢？

A <br>
只有等于0会显示为0, 哪怕是1 Drip 也会显示.
<br>

Q <br>
这个gas费是什么意思？所支付的gas费最终去了哪里？为什么有的转账所需要的费用特别多，有的少，多出来的去了哪里？

A <br>
发送交易需要矿工打包执行，gas 费是付给矿工的，这样才会有人愿意运行节点，gas 支付多少根发送交易的 复杂度，交易期望执行时间有关。多出来的一般会退回，不同的链具体回退机制也不一样。

Conflux挖矿奖励有3部分

1.出块基础奖励

2.手续费（gas费）

3.抵押存储产生的利息

portal默认的gas price只有1Drip，1cfx=100000000000000000drip
<br>

Q <br>
W/System.err: java.lang.RuntimeException: "\"transaction epoch height 0 is out side the range of the current pivot height (7946694) bound, only 100000 drift allowed!\""

A <br>
epochHeight 没有设置或设置的不对。option 里会自动设置 ，rawTx 不会自动设置。
<br>

Q <br>
错误返回码的明确对应关系表

A <br>
https://github.com/MetaMask/eth-rpc-errors/blob/84e90eb3ab121538eee406a67007cacb906c3fb9/src/error-constants.ts
<br>

Q <br>
FC怎么在shuttleflow上跨出来到以太坊

A <br>
FC是链内资产，目前不支持跨出到以太坊
<br>

Q <br>
zero one的输入法聊天内容加密后上链么？内容多了，会不会对资源造成很大的消耗

A <br>
非对称加密，没上链
另外消息上链存的是events，不是storage。
<br>

Q


A


Q


A


Q


A



