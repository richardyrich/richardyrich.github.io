---
layout: post
title: CFA Level 2 衍生 Part 1
categories: CFA2级笔记
---

## 目录

1. 远期合约（forward contract）
2. 期货（future）
3. 期权（option）
4. 离散时间期权定价：二差树模型（discrete-time pricing: the binomial model）
5. 连续时间期权定价：布莱克-休斯-墨顿模型（continuous-time pricing: Black–Scholes–Merton model）
6. 掉期合约（swap）
7. 货币掉期合约（currency swap）
8. 权益掉期合约（equity swap）

<br><br>

## 1\. 远期合约（forward contract）

<br><br>

远期合约的支付价格（forward price）
- 在交割期（settlement date）执行交易的价格
- 合理的远期合约的支付价格应该使得合约设定之初的价值（value）为零

远期合约的支付价格的无套利原则（non-arbitrage principle）

- 拥有相同现金流的两个产品应该有相同的定价

远期合约支付价格的定价

- 标的资产物（underlying asset）的现货价格（cash price） + 持有成本（carrying costs） + 持有收益（carrying benefits）
- S<sub>0</sub> × ( 1 + R<sub>f</sub> )<sup>T</sup>
- 持有收益可以便利收益率（convenience yield），或者股利，息票，利率等等
- 持有成本可以是标的资产物的储存和保险费用（一般指实物资产）

远期合约的价值（valuation）

V<sub>long</sub> = S<sub>t</sub> - forward price / ( 1 + R<sub>f</sub> )<sup>( T - t )</sup>

-----

### 特殊情况

权益远期合约（equity forward contract）

- 考虑到股利（dividend）的影响
- 权益远期合约的价格
  - = ( S<sub>0</sub> - <u>**PVD<sub>0</sub>**</u> ) × ( 1 + R<sub>f</sub> )<sup>T</sup>
- 权益远期合约的价值
  - = S<sub>t</sub> - <u>**PVD<sub>t</sub>**</u> - forward price / ( 1 + R<sub>f</sub> )<sup>( T - t )</sup>

债券远期合约（coupon bond forward contract）

- 息票（coupon）相当于股利，和权益远期合约的计算方法相同

指数远期合约（equity index forward contract）

- 假设：以无风险利率连续复利（continuously compounded risk-free rate）
  - R<sup>c</sup><sub>f</sub> = ln( 1 + R<sub>f</sub> )
- 指数远期合约的价格
  - = S<sub>0</sub> × e<sup>( R<sup>c</sup><sub>f</sub> - δ<sup>c</sup> ) × T</sup>
- 权益远期合约的价值
  - = ( S<sub>t</sub> / e<sup>δ<sup>c</sup> × ( T - t )</sup> ) - ( forward price / e <sup>R<sup>c</sup><sub>f</sub> × ( T - t)</sup>)

-----

远期利率协议（forward rate agreement (FRA)）

- 利率远期合约
- 交易量最大的远期合约
- 远期利率协议的“价格”就是远期利率

汇率远期合约（currency forward contract）

- 利率抛补平价（covered interest rate parity）

信用风险（credit risk）

- 交易对手风险（counterparty risk）
  - 远期合约价值为负的一方存在违约的可能性
  - 所以，远期合约价值为正的一方存在违约风险

盯市（marked to market）可以有效降低违约风险

<br><br>

## 2\. 期货（future）

<br><br>

远期合约vs期货

- 期货的本质就是远期合约
- 交易地点不同
  - 远期合约在场外交易（over-the-counter）
  - 期货在交易所交易，所有投资者的对家是清算所（clearing house）
- 期货存在盯市（mark to market）

远期合约的价格vs期货的价格

- 理论上两者应该相等
- 由于盯市的存在，实际上可能会发生偏离
  - 因为期货存在盯市，所以盈利可以立即取出，用于再投资
  - 当利率水平和标的资产物的价格存在正相关，期货的价格会比远期合约高
  - 如果负相关，期货的价格会比远期合约低



正向套利（cash and carry arbitrage）和反向套利（reverse cash and carry arbitrage）

- 利用标的资产物和期货之间存在的定价错误，做多一方的同时做多另一方，获得收益

正向市场（contango） vs 反向市场（backwardation）

- 正向市场：期货价格 > 现货价格
- 反向市场：期货价格 < 现货价格
- 期货溢价（normal contango）：期货价格 > 到期日（settlement date）现货的期望价格（expected cash price）
- 现货溢价（normal backwardation）：期货价格 < 到期日现货的期望价格

期货每天的盯市相当于重置期货的价值，重新回到0

期货的种类

- 短期国债期货（T-bill future）
- 欧洲美元定期存款单期货（eurodollar future）
  - 欧洲美元 = 离岸美元（offshore dollar）
  - 使用的贷款利率是LIBOR
- 长期国债期货（T-bond future）
  - 标的资产物为多个期限不小于期货制定的期限的长期国债
  - 因此做空方存在交割选择权（delivery option），每个作为标的资产物的债券都有一个相对应的转化因子（conversion factor (CF)）
  - 目的是为了防止逼仓（corner the market）：操作期货价格
- 货币期货（currency future）

<br><br>

## 3\. 期权（option）

<br><br>

和期货的区别是，期权是一个权利（right）而不是义务（obligation）

- 期权卖方（option writer）vs 期权买方（option holder）
- 看涨期权（call option）vs 看跌期权（put option）
- 期权价值等于期权价格（option price / option premium）

买卖权平价关系（put-call parity）

- c + X / ( 1 + R<sub>f</sub> )<sup>T</sup> = p + S<sub>0</sub>
- 看涨期权 + 无风险贴现债券（risk-free discount bond）= 看跌期权 + 现货价格（S<sub>0</sub>）
- 信托性买权（fiduciary call） = 抛补卖权（protective put）

<br><br>

## 4\. 离散时间定价：二差树模型（discrete-time pricing: the binomial model）

1. 股票二差树
2. 利率二差树

**注意：这里的例子使用的都是欧式期权，美式期权和百慕大期权要考虑提前行权的情况**

<br><br>

### a. 股票二差树

（假设利率不变）

看涨期权价值 = [ 风险中性上行概率 π × 股票上行时看涨期权价值 c<sup>+</sup> + ( 1 - 风险中性上行概率 π ) × 股票下行时看涨期权价值c<sup>-</sup> ] / ( 1 + R<sub>f</sub> )

- 风险中性上行概率 π = ( 1 + 无风险利率 R<sub>f</sub> - 下行幅度 d ) / ( 上行幅度 u - 下行幅度 d )
- 因为d < 1 + R<sub>f</sub> < u, 所以 0 < π < 1

看跌期权的逻辑相同

### b. 利率二差树

如果标的资产物（如，债券）和利率直接相关，则使用利率二差树
- 利率的变化将会是题目已知条件，不需要计算
- 上涨概率和下跌概率都是0.5

使用利率期权进行利率封顶（caplet）vs 利率封底（floorlet）vs 利率两头封（interest collar）

- 主要适用于浮动利率支付方（float rate payer）
- 利率封顶（caplet）：使用一系列的看涨期权，用于预防利率过高的情况
- 利率封底（floorlet）：相反，同理
- 利率两头封（interest collar）用在抵消使用期权的成本，既限制了潜在的风险，也牺牲了潜在的收益，目的是为了降低购买期权的花费

<br><br>

## 5\. 连续时间期权定价：布莱克-休斯-墨顿模型（continuous-time pricing: Black–Scholes–Merton model）

<br><br>

布莱克-休斯-墨顿模型假设：

- 价格变化符合对数正态分布（lognormal probability distribution）
- 无风险利率已知并且保持不变
- 标的资产物（underlying asset）的波动性已知
- 不存在税收和交易成本
- 标的资产物不存在现金流
- 使用的是欧式期权（european option）

布莱克-休斯-墨顿模型的自变量变化和期权价值的关系

- 标的资产物的价格变化（delta）
  - 当标的资产物价格上涨时，看涨期权价值上升，看跌期权价值下降
- 波动率的变化（vega）
  - 当波动性变大时，期权价值上升
- 无风险利率的变化（rho）
  - 当利率上升时，看涨期权价值上升，看跌期权价值下降
- 期权有效期的变化（theta）
  - 随着期权逼近期限，期权的价值下降
  - 例外：欧式看跌极实值期权（deep-in-the-money）
- 执行价格（exercise price）
  - 执行价格越高，看涨期权价值越低，看跌期权价值越高

delta动态对冲（delta dynamic hedging）

- 当投资者预测未来确定期限内会出现重大股价变动，但是不确定变动的方向，可以使用delta动态对冲锁定投资组合的价格防止损失

看涨期权和看跌期权的delta

- 在数值上：看涨期权的delta总比看跌期权的delta + 1
- 看涨期权的delta变化：随着股价从 0 到 + ∞，delta从 0 到 1
- 看跌期权的delta变化：随着股价从 0 到 + ∞，delta从 -1 到 1
- 此外，其他条件保持不变，随着期权逼近期限（theta变化），delta也会发生变化

delta动态对冲（delta dynamic hedging）的特点

- delta中性投资组合（delta-neutral portfolio）：做多价值为n股票，则做空价值为n / delta 的看涨期权，或者做多价值为n / delta 的看跌期权
- delta中性对冲是一个动态的过程，因为delta不停的在变化

gamma动态对冲（gamma）

- gamma测量的是delta的敏感度
  - delta可以理解为标的资产物的价格的一阶求导，gamma是二阶求导
- 有相同的执行价格和期限的看涨期权和看跌期权有相同的gamma
- 做多看涨期权和看跌期权时，gamma都为正数
- 平价期权（at-the-money）的gamma最大，极实值期权（deep-in-the-money）和极虚值期权（deep-out-of-the-money）的gamma最小，趋近于0

波动性（volatility）

- 历史波动率（historical volitility）：使用布莱克-休斯-墨顿模型进行定价时的使用的波动率
- 隐含波动率（implied volatility）：由现有期权价格逆推出的隐含波动率

布莱克模型（Black model）

- 原理和布莱克-休斯-墨顿模型一样，只是标的资产物是远期合约或者期货
- 由该模型可得出，标的资产是期货时，美式期权比欧式期权价值高
  - 因为期货存在盯市，盈利可以即时变现
- 标的资产是远期合约时，美式期权和欧式期权价值一样

<br><br>

## 6\. 掉期合约（swap）

<br><br>

掉期合约（swap）

- 间隔相等，交换一系列的现金流
- 互换时点（settlement date），互换区间（settlement perid）
- 名义本金（notional value）是用于计算的，实际上本金没有发生交换
- 固定现金流（fixed leg）
- 浮动利率现金流（floating leg）
- 固定利率现金流（fixed leg）

单纯利率交换（plain vanilla interest rate swap）

- 浮动利率支付方（floating-rate / variable-rate payer）
- 固定利率支付方（fixed-rate payer）
- 每一次进行交换，现金支付是以钆差交收（netting）的形式进行交易，也就是说只支付差额
- 掉期合约的价格是固定利率支付方支付的利率

掉期合约的原理

- 可以理解为一系列的远期利率合约（forward rate agreement (FRA)），虽然这四个FRA的价格不一定为零，所以他们属于是场外（off the market）远期利率合约，但是加起来价格为0
- 可以理解为一系列的看涨期权和看跌期权
  - 因为看涨期权和看跌期权合起来就相当于期货

掉期合约的价格计算

- 一般题目给出每一次息票的折现因子（discount factor）
  - 折现因子 × 息票剩余价值 = 息票现值
- 由以下公式能够得出掉期合约的价格（也就是固定利率）
- C = ( 1 - Z<sub>n</sub> ) / ( Z<sub>1</sub> + Z<sub>2</sub> + ... + Z<sub>n</sub>)
- 将C**<u>年化后</u>**可获得掉期合约年利率

## 7\. 货币掉期合约（currency swap）

- 名义本金（notional principals）发生了交换
- 现金流可以是固定利率，可以是浮动利率，也可以混合

<br><br>

## 8\. 权益掉期合约（equity swap）

- CFA一般考察固定利率和权益收益之间的掉期