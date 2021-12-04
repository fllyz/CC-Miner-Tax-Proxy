## 下载

目录里的文件都要下载

## 运行方式①

打开CaoMinerTaxProxy.exe，记得关闭杀毒软件，不然可能误报
打开后几个配置自己配置，配置完了点击启动
每次启动系统都要重新运行一次

## 运行方式②

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

管理员权限打开命令行cmd
切换到本目录

输入nssm install CMinerProxy
点击Path后面的省略号，选择ccminertaxproxy.exe
点击Install service
重启系统即可自动启动


## 注意

如修改了配置，修改后需要重新执行程序，或者去services.msc里重启CMinerProxy服务
千万不要忘记修改配置文件

无法连接的记得开防火墙
