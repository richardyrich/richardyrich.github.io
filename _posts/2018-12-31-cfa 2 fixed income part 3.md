---
layout: post
title: CFA Level 2 固定收益 Part 3
categories: CFA2级笔记
---

## 目录
1. 可赎回债券和可卖回债券的分析和估值（续）
2. 有利率浮动上、下限的浮动利率债券（capped and floored floating-rate bonds）的估值和分析
3. 可转换债券（convertible）的估值和分析
4. 度量信用风险（measure of credit risk）
5. 传统信用评级（traditional credit rating）
6. 使用结构性模型（structural model）估算权益和债券价值
7. 信用利差的期限结构（term structure of credit spread）
8. 资产担保证券（asset back security）的信用分析


<br><br>

## 1\. 可赎回债券和可卖回债券的分析和估值（续）

<br><br>

（续上一部分）

### e）对于含权风险债券（risky bonds）的估值

期权调整价差（option adjusted spread）

- 考虑到风险债券存在违约风险，将先前的无风险债券的二差利率树的利率水平进行向上调整
- 零利率波动利差（zero-volatility spread / Z-spread）没有考虑到期权的影响，所以需要进行调整
- 这个调整后的上调的幅度，引入了一个新的名词，期权调整利差（option adjusted spread）
- 期权调整价差考虑到利率波动和内含期权的影响，计算的是实际利差

当利率波动性增加

- 可赎回债券的期权调整利差变小
- 可卖回债券的期权调整利差变大

### f）含权债券的利率风险（interest rate risk）

<br><br>

久期（duration）计量了债券对于利率变化的敏感度（包括应计利息（accrued interest））

> 久期在上一个部分简单提及了一下

久期可以分为两类

a. 收益率久期计量（yield duration measures）

- 修正久期（modified duration）
  - 仅用于无权债券，因为假设现金流不会因为利率变化而改变

b. 曲度久期计量（curve duration measure）

- 有效久期 / 期权调整后久期（effective duration / option-adjusted duration）
  - 可以用于直接债券和含权债券
  - 假设基准利率曲线仅发生平行移动
  - effective duration = [ ( PV<sub>-</sub> ) - ( PV<sub>+</sub> ) ] / [ 2 × ( △curve ) × ( PV<sub>0</sub> ) ]

可赎回债券的久期特点

- 总的来说
  - 内含期权会导致债券的有效久期减少

**可赎回债券**

- 当基准利率高时
  - 可赎回债券和非可赎回债券的有效久期很相似
- 当基准利率低时
  - 可赎回债券的有效久期比非可赎回债券的有效久期短

**可卖回债券**

刚好相反

单边久期（one-sided duration）
- 含权债券价格对于利率的增减的敏感度是不对称的（asymmetircal）
- 单边久期是含权债券在利率只增加，或者只下降的情况下计算出的有效久期
- 单边久期更好的度量了含权债券对于利率变化的敏感度，尤其是该债券趋于平值状态（near the money）

关键利率久期（key rate duration）

- 债券对于某个特定期限的敏感度
- 对于平价流通的（trading at par）**<u>不含权债券</u>**，仅有和其期限相等的（maturity-matching）关键利率久期不为0

可赎回债券

- 息票越高，赎回的可能性越大，导致有效久期越小
- 息票越低，赎回的可能性越低，导致该债券的表现和不含权债券类似，和其期限相等的关键久期最大

可卖回债券

- 息票越高，赎回的可能性越低，导致该债券的表现和不含权债券类似，和其期限相等的关键久期最大
- 息票越低，卖回的可能性越大，导致有效久期越小

有效凸性（effective convexity）

a. 直接债券

- 较低的正凸性
  - 幅度相同的情况下，利率下降比上升带来的价格影响更大

b. 可赎回债券

- 当基准利率较高时，出现正凸性
- 当基准利率较低时，出现负凸性

c. 可卖回债券

- 正凸度
  - 相比直接债券，可卖回债券更大

  <br><br>

## 2\. 有利率浮动上、下限的浮动利率债券（capped and floored floating-rate bonds）的估值和分析

<br><br>

存在利率上限的（capped floater）浮动债券有利于发行人

- 利率上限的浮动债券的价值
  - 直接债券的价值 - 浮动上限的价值

存在利率下限的（floored floater）浮动债券有利于持有人

- 利率下限的浮动债券的价值
  - 直接债券的价值 - 浮动下限的价值



## 3\. 可转换债券（convertible）的估值和分析

<br><br>

可转换债券（convertible）相关概念

- 转换价格（conversion price）
  - 可转换债券（convertible）行权时购买股票的价格
- 转换价值（conversion value）
  - = 标的股票价格（underlying share price）× 转换率（conversion ratio）
- 转换价值下限（minimum / floor value of a convertible bond）
  - = 转换价值，或者至少不小于相似直接债券的价值
- 市场转换价格（market conversion price）
  - **<u>注意和转换价格（conversion price）区分</u>**
  - = 转换债券价格（convertible bond price） / 转换率（conversion ratio）
  - 实际的转换价格（放弃的债券带来的机会成本 / 股份数）
- 每股市场转换溢价（market conversion premium per price）
  - = 市场转换价格（market conversion price） - 标的股票价格（underlying share price）
  - **和常见的溢价相反：成本 - 收益**
- 市场转换溢价比率（market conversion premium ratio）
  - = 每股市场转换溢价 / 标的股票价格（underlying share price）
  - **和常见的收益率相反：成本 / 收益 - 1**
- 溢价比率（premium over straight value）
  - = 转换债券价格（convertible bond price） / 相似直接债券价值 - 1
  - 可转换债券的价值相当于直接债券和股票看涨期权之和，溢价比率计算的是看涨期权的价值占比

可转换债券（convertible）的估值

- 当转换价格（conversion price）明显高于股价时
  - 被称为直接债券等价物（bond equivalent），或垃圾可转债（“busted convertible”）
  - 此时转换债券几乎不存在转换价值
  - 那些常规上能影响直接债券的收益率因素，如信用风险，利率风险等，也以相似的方式影响垃圾可转债
  - 股票价格几乎不影响垃圾可转债的价值
- 当转换价格明显低于股价时
  - 被称为股票等价物（stock equivalent）
  - 此时转换债券的价值几乎等于转换价值（follow the conversion value closely）
  - 转换债券的价值与股票价格关系密切（exhibit mostly risk-return characteristics）
  - 那些常规上能影响直接债券的收益率因素对此时的可转换债券价值影响不大
- 当转换价格高于股价，但股价在逐步接近转换价格（上升）时
  - 转换债券的价值动态与股票价格动态比较接近，但比股票的价格上升幅度小
- 当转换价格低于股价，但股价在逐步接近转换价格（下跌）时
  - 转换债券的价值动态与股票价格动态比较接近，但比股票的价格下降幅度小

<br><br>

## 4\. 度量信用风险（measure of credit risk）

<br><br>

相关概念

- 违约概率（probability of default）
- 违约损失率（loss given default）
  - 违约后损失的百分比
  - 恢复率（recovery rate）= 1 - 违约损失率
- 期望损失（expected loss）
  - 违约概率 × 违约损失率
- 期望损失的现值
  - 使用风险中性概率（risk-neutral probability）
  - 考虑 到货币的时间价值（time value of money）
  - **期望损失的现值 = 无风险债券价值 - 风险债券的价值**
  - 风险中性期望损失的现值和期望损失之间的大小不确定

-----

风险中性期望损失的证明过程：

> - 必要收益率 = 无风险利率 + 风险溢价
> - 那么，如果假设风险中性 - > 风险溢价 = 0

#### 1）证明：期望收益 = 1 - 期望损失

假设1年期无息债，剩余价值为 $100

- 违约（概率 = 违约概率）
  - 收益 = 违约概率 × $100 ×（1 - 违约损失率）
- 无违约（概率 = 1 - 违约概率）
  - 收益 =（1 - 违约概率）× $100

所以，期望收益

- = 违约概率 × $100 ×（1 - 违约损失率）+（1 - 违约概率）× $100
- 化简 = $100 - 违约概率 × 违约损失率 = **<u>$100 ×（1 - 期望损失）</u>**

#### 2）证明：期望损失 ≈ 持有期收益率 - 无风险利率

假设投资者风险中性，那么对于此风险债券的必要收益率 = 无风险利率，也就意味着：

- $100 ×（1 - 期望损失）/ 现值 = 1 + 无风险利率

也就是说：现值 = $100 ×（1 - 期望损失）/（1 + 无风险利率）

同时，依照定义：现值 = $100 × 1 /（1 + 持有期收益率）

所以，（1 - 期望损失）/（1 + 无风险利率）= 1 /（1 + 持有期收益率）- > 期望损失 ≈ **<u>持有期收益率 - 无风险利率</u>**

#### 3）证明：风险中性期望损失 > 期望损失

持有期收益率 - 无风险利率 = 信用利差 + 流动性利差

因为风险中性期望损失还包含了流动性风险，而一般意义上的期望损失只包含信用风险，所以

- 所以**<u>风险中性期望损失 > 期望损失</u>**

-----

<br><br>

## 5\. 传统信用评级（traditional credit rating）

- 信用评分（credit scoring）
  - 用于小企业及个人
- 信用评级（credit ratings）
  - 用于公司，政体，资产担保证券（asset back security）
  - 评价机构由被评估对象支付运营费用，所以存在一定的利益冲突
  - 评价机构可能倾向于保持原有评级，避免造成波动

<br><br>

## 6\. 使用结构性模型（structural model）和简约型模型（reduced form model）估算权益和债券价值

<br><br>

### 结构性模型（structural model）

- 依靠公司的负债经济情况（economics of a company's liabilities）和期权定价理论（option pricing theory）
- 结构性模型注重于公司的资产负债表，而得其名

公司的股东的责任有限

- 持有公司的权益相当于持有公司资产的看涨欧式期权
- 当公司资产的价值 > 负债的价值，存在违约风险，股东价值为0
- 当公司资产的价值 < 负债的价值，股东的价值等于总资产减去总负债的剩余

公司债权人的有优先权偿付权

- 成为公司的债权人相当于持有公司资产的看跌欧式期权
- 执行价格为债券期限，执行价格为债券面值

结构性模型的假设（本质是布莱克-休斯-墨顿模型）

- 公司的资产在无摩擦，无套利机会的市场（frictionless markets that are arbitrage free）中交易
- 无风险利率水平恒定
- 公司资产的时间价值（time value）表现出对数正态分布（lognormal distribution），平均值为μT，方差为σ<sup>2</sup>T

结构性模型的公式（如果满足以上假设）

- 股东的权益价值
  - S<sub>t</sub> = A<sub>t</sub> N (d<sub>1</sub>) - K e <sup>-r ( T - t )</sup> N (d<sub>2</sub>)
- 债权人的债权价值
  - D<sub>( t, T )</sub> = A<sub>t</sub> N (- d<sub>1</sub>) + K e <sup>-r ( T - t )</sup> N (d<sub>2</sub>)
- 其中
  - d<sub>1</sub> = [ ln( A<sub>t</sub> / K ) + r ( T - t ) + 1/2 × σ<sup>2</sup>( T - t ) ] / [ σ × ( T - t )<sup>0.5</sup> ]
  - d<sub>2</sub> = d<sub>1</sub> - σ × ( T - t )<sup>0.5</sup>

此时违约概率（probability of default）= N(d<sub>1</sub>)

将结构性模型公式进行改进

- 将该公式中进行修改就可以计算实际的违约损失（考虑到投资者不是风险中性而是风险厌恶的），将公式中的无风险利率改成实际利率即可：r - > μ
  - 其中 e<sub>1</sub> = [ ln( A<sub>t</sub> / K ) + μ ( T - t ) + 1/2 × σ<sup>2</sup>( T - t ) ] / [ σ × ( T - t )<sup>0.5</sup> ]
  - 其中 e<sub>2</sub> = e<sub>1</sub> - σ × ( T - t )<sup>0.5</sup>

所以，实际期望损失 = K N( -e<sub>2</sub> ) - A<sub>t</sub> e<sup>μ( T - t )</sup> N ( - e<sub>1</sub> )

期望损失的现值 = 无风险债券价值 - 风险债券的价值 = K P(t, T) - D(t, T) = K e <sup>-r ( T - t )</sup> N ( - d<sub>2</sub> ) - A<sub>t</sub> N ( - d<sub>1</sub> )

结构性模型的优劣

优点

- 利用了期权模型模拟了公司的违约概率
- 仅需使用当前市场数据

缺点

- 仅使用资产负债表数据，并不考虑宏观的经济周期（business cycle）
- 仅能使用隐含估计确定参数数值，因为公司实际的资产价值不易知晓，而布莱克-休斯-墨顿模型存在缺陷
- 布莱克-休斯-墨顿模型的三个前提假设并不符合实际

<br><br>

### 简约型模型（reduced form model）

- 假设公司的零息票债券在无摩擦，无套利机会的市场中交易
- 无风险利率，r <sub>t</sub>，是随机的（stochastic）
- 经济情况的变化可以使用不同的随机（stochastic）变量 X<sub>i</sub> 表示
- 在不同的经济情况，违约概率用 λ(X<sub>i</sub>) 表示
- 在违约情况下，违约损失率为 t(X<sub>i</sub>) 表示

简约型模型的优劣

优点

- 公式的自变量都是可以在市场中观察可得，所以可以使用历史数据
- 相对于结构性模型
  - 考虑到了经济周期的变化（business cycle）
  - 不需要考虑公司的资产债务结构

缺点

- 风险率估计（hazard rate estimation）使用的是历史数据，所以模型应该合理（properly formulated）并且通过事后检验（back test）


### 两种确定期权定价模型中参数的数值（estimate the parameters）的方法

- 【仅简约型模型可以使用】历史估计（historical estimation），又名，风险率估计（hazard rate estimation）
  - 因为现实生活中不存在无摩擦市场，所以历史数据并不隐含数据有效
- 【结构型模型和简约型模型都可以使用】隐含估计（implicit estimation），又名，调整（calibration）
  - 根据期权本身的价格推算出来


<br><br>

## 7\. 信用利差的期限结构（term structure of credit spread）

<br><br>

信用利差的期限结构表示的是零息票无风险收益率和零息票风险债券收益率之间的利差

步骤

1. 估算含息票风险债券的价值
2. 通过含息票无风险债券的收益率，推算出折现因子（discount factor）
  - 因为期限超过一年的国债不发息票的较少
3. 计算零息票风险债券的收益率
  - 使用的是连续利率水平，D (t, T) = e <sup>-y<sub>D</sub> (t, T) (T - t)</sup>
4. 计算零息票无风险债券的收益率
  - 使用的是连续利率水平，P (t, T) = e <sup>-y<sub>P</sub> (t, T) (T - t)</sup>
5. 相减算出信用利差

期望损失的现值


## 8\. 资产担保证券（asset back security）的信用分析

- 资产担保证券（asset back security）的信用分析涉及到抵押资产池（collateral pool）和收益的分配顺序（distribution waterfall）
- 可以使用结构性模型或者简约型模型（reduced form model）
- 信用风险指标（credit risk measures）
  - 损失概率（probability of loss）
  - 期望损失（expected loss）
  - 期望损失的现值（present value of expected loss）
