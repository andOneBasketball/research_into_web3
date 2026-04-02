# 小白入门就看这个
这一篇会持续更新，然后尽可能的保持精简

## Web3黑暗森林法则
🔴 这个非常重要，刚了解web3的你可能感知还不强，你可以先读完全文再回过头来好好看 web3黑暗森林法则。然后文章比较长读起来对于小白来说相对费劲。但它是在web3圈内行走需要时刻谨记的东西。[Web3黑暗森林法则](https://github.com/slowmist/Blockchain-dark-forest-selfguard-handbook/blob/main/README_CN.md#aml)

## 区块链
简单理解，每条链可以类比为不同的银行，在交通银行肯定不能直接看到招商银行的存款。
每个区块会记录很多笔交易数据，区块和区块连接在一起就是区块链

## 钱包部分
web3 的钱包分为托管钱包和非托管钱包，托管钱包私钥（可以是助记词，也可以是一段字符串私钥）掌控在自己手里

### 非托管钱包
我通过工具生成了一个钱包，私钥是 3aa09f0563e033c1c34471a011ac52b8a3d46845578d284c3e6bb5ff42320914，将该私钥导入到任意钱包 app（metamask、imtoken、Trust Wallet） 都可以加载出该钱包的余额
分享一个在线生成钱包的站点 [https://iancoleman.io/bip39/#english](https://iancoleman.io/bip39/#english)，但不保证该站点不会记录用户生成的私钥数据

##### 将钱包私钥导入到metamask
将钱包的私钥导出留作分享后的小作业，自行实操体验
![meatmask私钥导入](./img/metamask1.gif)

##### 助记词钱包导入到metamask
我通过工具生成了一个钱包，助记词是 ostrich sting tuna tag broccoli purpose world rich thing rule couch abstract differ record radar rival rapid rack dirt slab move east student purse，将该助记词导入到任意钱包 app（metamask、imtoken、Trust Wallet） 都可以加载出该钱包的余额
![meatmask助记词导入](./img/metamask2.gif)

##### 将 Custom 链导入到钱包内
区块链节点查询 https://chainlist.org/?testnets=true
钱包通过 rpc 节点调用链上合约公开的 协议接口 获取到用户的资产数据
![meatmask导入 Custom 链](./img/metamask3.gif)

##### 将代币导入到钱包内
https://coinmarketcap.com/中记录各种基于共识的代币数据，例如 USDT，coinmarketcap 记录了 USDT 在各条链上发行的代币地址，将代币地址导入钱包内
![cmc](./img/cmc.gif)

### CEX
各大交易所（OKX、Binance、Gate.io）实际都是托管钱包，用户可以在各大交易所通过 C2C 交易使用法币换 OTC 商家的数字货币。

#### C2C 交易
以下是 Binance C2C 交易的教程，注意在C2C 交易过程中一定要识别 卖家的实名和 币安 C2C 交易中商家的实名一致
[https://www.binance.com/zh-CN/blog/c2c](https://www.binance.com/zh-CN/blog/c2c/7428324997079645557#%E5%B8%81%E5%AE%89-C2C-%E6%96%B0%E6%89%8B%E6%8C%87%E5%8D%97%E5%A6%82%E4%BD%95%E5%AE%89%E5%85%A8%E4%B9%B0%E5%8D%96%E5%8A%A0%E5%AF%86%E8%B4%A7%E5%B8%81)

#### 提币
🔴 千万注意别提错链了

##### Binance
通过法币购买数字货币后，可以在交易所将代币提币到链上。
提币到链上可以选择提取链原生代币（例如 BSC 链则选择提币 BNB，以太坊链则选择提币 ETH）到链上，再在链上的 DEX 将原生代币换成其他数字货币（例如 USDT、USDC）。
![binance](./img/binance1.png)

##### OKX
OkX 由于提币的资产界面禁止截屏，提取数字货币到链上按照以下步骤
提币 =》选择资产 =》选择地址簿或者非托管钱包 =》选择网络 =》输入地址

#### 区块链浏览器
将代币地址输入到区块链浏览器中，就能获取到该代币的相关数据（包括代币信息，该代币涉及的交易数据）
例如以下链接是 BSC 链的区块链浏览器，其他链的可自行在 Google 搜索访问
* [https://bscscan.com/](https://bscscan.com/)
* [https://bscscan.com/address/0x55d398326f99059ff775485246999027b3197955](https://bscscan.com/address/0x55d398326f99059ff775485246999027b3197955)

### DEX
去中心化交易所，将 CEX 中的代币提币到 链上后，可以在 DEX 内交换出你想要的代币。在代币中输入代币地址即可匹配到对应的代币，代币的共识地址可以在 ![coinmarketcap](https://coinmarketcap.com/) 中查询
* [uniswap](https://app.uniswap.org/)
* [pancakeswap](https://pancakeswap.finance/swap)
![uniswap](./img/uniswap.gif)

### 代币水龙头
- POL 测试网关代币水龙：[https://faucet.polygon.technology/](https://faucet.polygon.technology/)
- Sepolia 挖矿，消耗PC资源，风扇呼呼转：[https://sepolia-faucet.pk910.de/](https://sepolia-faucet.pk910.de/)
- BSC 测试网代币水龙头：[https://www.bnbchain.org/en/testnet-faucet](https://www.bnbchain.org/en/testnet-faucet)，需要主网的钱包BNB 余额 0.002 BNB
- Chainlink 上有各个网络的代币水龙：[https://faucets.chain.link/](https://faucets.chain.link/)，大多需要以太坊主网的余额 1 LINK


## 贡献者
期望更多的贡献者加入项目，这个列表会持续更新，希望你有任何的想法也联系我：
0xFork，Twitter (@0xSevenK)