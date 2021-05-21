---
description: Testnet
---

# 机枪池及BNB/HT质押挖矿

机枪池

OFT将会在机枪池开放后的一个月内每个区块释放200 OFT，之后的每个月都会根据OFT市价以及通缩模型动态调整后在每个BSC区块内释放低于200的 OFT

### 运行机制：

![](../.gitbook/assets/image%20%284%29.png)

* 选择全网最高收益率及安全性最好的交易对
* 智能合约自动进行每日复投
* 根据市场风险和收益率变化自动新增或下架新的流动性质押交易对

### 用户收益（以Pancakeswap为例）：

* 70%的流动池挖矿收益将会以该流动池的奖励发放
* 30%的奖励将以OFT形式发放
* 由于OFT的通缩机制以及用户增长，OFT本身的价值会比用户直接在原生平台质押流动性获取更多的收益（15%以上年化）

### 机枪池套利

* 根据用户奖励机制及OFT区块发放，交易通缩等机制，OFT交易用户实际上可以计算出OFT的买盘价格，并根据实时价格计算来进行套利

## 原生单币挖矿



### BNB Validator staking:

架构:

![](../.gitbook/assets/image%20%282%29.png)

**Bite** the sweet sizzling juicy yields on top of the well sliced "onions" !!

* 根据币安数据，去年的节点平均奖励年化是60%
* 币安智能链的21个节点奖励分配比例在80%至50%之间
* Onion Farm会动态调节节点锁仓，保证赚取最大的奖励年化
* 币安智能链目前交易量已经超过ETH
* 智能合约安全质押锁仓，保证用户资金安全和可兑换性
* 币安智能链的质押解锁期 - **7 days**

我们的第一个矿池将会使用 BNB 并在BSC上部署相应的智能合约，同时给与用户一定量的OFT来最大化用户收益

我们的另外一个优势是能够实现更短的BNB质押解锁期：

{% page-ref page="../introduction/mechanism/redeem.md" %}

## HECO Tinder Pool

{% hint style="info" %}
_The project will start with BNB for a start, before expanding into other assets. The main reason is that Heco Node Election is not completed yet._
{% endhint %}

* Miners pledge HT to become one of the 21 validator nodes or 11 backup nodes
* stakers delegate their HT to Miners and share 70%~100%% Miner rewards
* Dynamic yield maximizing across multiple validators
* Easy unstaking by sending  an unstake transaction to the **Validators Contract** and only wait for 86400 blocks to withdraw all staked assets

### ETH Specific features

i.e. for Ether staking:

* Dynamic yield maximizing across multiple validators
* Early unlock from staking
* ETH 2.0 POS
* So many ether hodlers sleeping in those saving scheme or in exchanges

The project will start with BNB on BSC network in a short while after product goes live, before expanding into other BSC assets with mining/lending

