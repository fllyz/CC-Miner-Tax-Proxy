## 更改权限

``` bash
$ chmod a+x ccminertaxproxy
```

## 编辑配置

自行编辑config.json文件
``` json
{
  "poolAddress": "eth.f2pool.com",//矿池域名或者IP
  "poolPort": 6688,//矿池端口
  "tcpPort": 6688,//中转的TCP模式端口
  "tlsPort": 12345,//中转的SSL模式端口
  "user": "你的钱包地址",//你的钱包地址，或者你在矿池的用户名
  "worker": "矿工地址",//容易分辨的矿工名
  "taxPercent": 0.35//抽水百分比，单位%，只能输入0.3-20之间的数字
}
```

## 运行

``` bash
$ ./ccminertaxproxy
```

## 自启动

自己想办法吧，systemctl，supervisor啥的都行