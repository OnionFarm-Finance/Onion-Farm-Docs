# 彩票池规则 1.0

### 彩票合约地址

{% embed url="https://testnet.bscscan.com/address/0x516ffd7D1e0Ca40b1879935B2De87cb20Fc1124b" caption="" %}

**合约细则:**

* **彩票池的资金主要来源于用户彩票购买使用的OFT，上一轮奖池转入以及OFT自有的通缩式交易费用\(0.5%\)** 
* 每张彩票价格固定为: 100 OFT
* 单一用户彩票购买限额: 没用总限额, 但是在彩票UI内一次性只能购买50张彩票
* 购买一张彩票后用户会获得一个随机产生的四个数字组合的NFT。每个数字范围是1-14, 比如用户会随机获得 “1-9-3-2”

\*\*\*\*

**赢取规则:**

如果想赢取奖励, 用户获得的四位随机数彩票需要能够完整按顺序对应本期彩票大奖结果

如果你的彩票没有能够全部投中，那也无需担心。只要你中两个或者三个数字，也会赢得相应的二三等奖

**Winning Ratio:**

* 四位数字按顺序全中 = 获得或分享奖池内50% 的OFT
* 三位数字按顺序投中 = 赢取或分享奖池内10%的OFT
* 两位数字按顺序投中 = 赢取或分享奖池内5%的OFT
* 奖池智能合约将会燃烧奖池内剩余的 15% OFT, 并将剩余20% OFT转入下一轮奖池

Please note - 如果本轮一等奖，二等奖或者三等奖无人中奖，那么对应的OFT奖池分配额度将会40%燃烧，60%累积至下一轮奖池

For example, if the final 4 winning numbers are “1-9-3-2”:

* “2-3-9-1” = match 0
* **“1-9-3-2” = match all 4**
* “1-9-2-2” = match 3
* “2-3-3-2” = match 2
* “1-2-1-2” = match 2

**彩票运行示例:**

**Phase 1 - 购买彩票 \(1 PM to 2 PM\)**

* 每轮彩票池开放后用户有一小时来购买彩票 
* 奖池会根据用户购买数来更新奖励规模
* 用户购买后会收到一张带有四位数字信息的NFT彩票 \(comprised of 4 digits\) for each 100 OFT paid.

**Phase 2 - 彩票开奖! \(2 PM\)**

* The 4 winning lottery numbers are drawn and will appear on the page. 
* Each participant’s winnings will be automatically calculated based on their ticket numbers and shown on the page.
* Users can claim winnings if they have any.
* Users will also be able to see the lottery results: How many users matched all 4 numbers, 3 numbers and 2 numbers. 

**Phase 3 - 兑现 \(2 PM - 3PM\)**

如果你赢取了奖励，可以在兑现界面兑换相应的NFT奖励

下一轮奖池会在三点后重新开放

## **How are ticket numbers drawn?**

The lottery aims to be completely random. Even though the ticket numbers given out are determined by a front-end logic, there is an extremely low chance that anyone is able to determine the 4 winning numbers ahead of time.

* 第一个中奖数字将会根据参与奖池的用户数字与一小时内的区块hash来确定 lottery number will be determined based on the %10 remainder of a hash encoded by the blockhash and the number of participating users at the entry deadline.
* The 2nd lottery number will be determined based on the %10 remainder of a hash encoded by the blockhash and the total pooled cake balance at the entry deadline.
* The 3rd lottery number will be determined based on the %10 remainder of a hash encoded by the blockhash and the timestamp of the last lottery participant at the entry deadline.
* The 4th lottery number will be determined based on the %10 remainder of a hash encoded by the blockhash and the block difficulty at the entry deadline.

