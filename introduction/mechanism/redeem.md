# BNB 解锁

## Redeeming HT or BNB

📍 持有 oBNB or oHT 的用户可以兑换BNB, 根据 LBNB/BNB 兑换率。币安支持的质押解锁期是7天，但是根据我们的预期，由于新用户不断质押和解锁，这个周期是可以缩短的。

{% hint style="info" %}
The unbonding process of BNB is a fixed 7 days for direct Binance Chain\(BC\) Validators.

HT Validator unstaking process should be more or less the same
{% endhint %}

用户数量增长后，会有更多用户去申请提前解锁，也会有更多用户申请质押。这样质押和解锁的需求可以在智能合约内进行一些对冲，允许用户在少于七天的时间里解锁（一般为2~3天）

举例:  
_如果用户A想要质押 100 BNB，用户B想要解锁70 oBNB，那用户B可以得到全部质押解锁_ 

_反过来，如果用户A想要质押 70 BNB，用户B想要解锁100 oBNB，那用户B只能暂时解锁70 BNB并将剩余的30 oBNB放入解锁队列_

_另外，智能合约将会保证所有满足币安七天解锁期的用户得到完全解锁，而不是放入解锁池中供其他用户解锁_

