---
layout: post
title: CFA Level 2 固定收益 Part 1
categories: CFA2级笔记
---


## 目录

1. 即期利率（spot rate）vs 远期利率（forward rate）
2. 掉期利率曲线（swap rate curve）
3. 利率的期限结构的传统理论（traditional theories of the term structure of interest rates）
4. 现代期限结构模型（modern term structure model）
5. 收益率曲线因子模型（yield curve factor models）
6. 小结

<br><br>

## 1\. 即期利率（spot rate）vs 远期利率（forward rate）

<br><br>

**零息债券即期收益率（spot rate）**

- 无风险（risk-free）单次支付的（single-unit payment）债权的到期收益率（yield to maturity）

零息债券即期收益率曲线（spot curve）

- 将不同期限的零息收益率绘制在一张表上形成的曲线
- 在CFA Level 2 中又被成为收益率曲线（yield curve）
- 贴现因子（discount factor）
	- 将特定期限的无息债权折现至现值的折现率

> 在CFA Level 1 中，yield curve表示的是不同期限的债权的持有期收益率（yield to maturity (YTM)）的曲线

**无套利零息远期利率（arbitrage-free forward rate）**

- 未来特定时刻的零息债券即期收益率
- 相关的两个表示符号，f(T\*,T)和F(T\*,T)
	- f(2,3)表示两年后的三年期限的零息债券的年化利率
	- F(3,2)表示三年后的两年期限的零息债券的价格
	- F(T\*,T) = 1 / ( 1 + f(T\*,T) )<sup>T</sup>

零息债券远期收益率模型（forward rate model）

- ( 1 + r(T\*,T) )<sup>(T\* + T)</sup> = ( 1 + r(T\*) )<sup>T\*</sup> ( 1 + f(T\*,T) )<sup>T</sup>
- 这是一个逆向归纳法（backward induction valuation）的一个简单的运用

**即期利率曲线（spot curve）vs 远期利率曲线（forward curve）**

- 向上倾斜的即期利率曲线（r(T\* + T) > T(T\*)
	- 远期利率曲线总在即期利率曲线之上
	- T\*值越大，远期利率越高
- 向下倾斜的即期利率曲线（r(T\* + T) < T(T\*)
	- 正好相反

平价收益率曲线（par curve）

- 平价发行的（priced at par），付息国债（coupon-paying government）的到期收益率（yield to maturity）曲线
- 绘制零息债券即期收益率（spot rate）前，需要使用平价收益率曲线
	- 计算过程需要用到拔靴/自助（bootstrapping），这是一个正向替代模型（forward substitution）


到期收益率（yield to maturity）的三个前提假设：

- 债权持有至到期日（maturity）
- 所有的本金和息票都全额获得（made in full when due），不存在违约情况
- 持有期间所有的息票都能以原有的到期收益率再投资（reinvested at the original YTM）

实际报酬率（realized return / horizon yield）

- 投资者实际的收益，并进行年化计算

### 结论1：

如果当前的远期利率（forward rate）是未来利率的准确估计，那么远期合约的价格（forward contract price）将保持不变

- 所以远期合约的价格变化意味着实际利率和过去的远期利率预测发生偏离

### 结论2：

如果即期利率都能被远期利率准确预测，那么不同期限的债权的在相同的时期内的持有期收益率（holding period return）是一样的

- 该结论是 **到期日匹配策略（maturity matching strategy）** 的理论基础
- 买入到期日和投资期限相匹配的债权的投资战略

### 结论3：

如果在未来，即期利率和历史的远期利率不一致，投资者在到期日之间交易就会造成收益或者损失

- 如果投资者预测未来的即期利率曲线比远期利率曲线低，可提前售出获得高出无风险利率更高的收益



### 结论4：

骑乘收益率曲线（riding / rolling down the yield curve）

- 如果投资者认为市场的远期利率曲线对未来的即期利率进行了高估，可通过交易比投资者的投资期限更长的债权获取更高的收益
	- 该策略比到期日匹配策略（maturity matching strategy）收益高

### 结论5：

如果未来即期利率低于预期，应该买入远期合约

### 小结：

- 如果投资者认同远期利率对于未来即期利率的预测
	- 债券市场不存在不确定性
	- 使用 到期日匹配策略（maturity matching strategy）是最佳的投资方式
	- 使用 骑乘收益率曲线（riding / rolling down the yield curve）策略 只会让交易更频繁，而且收益率并不会更高
- 如果投资者认为远期利率对于未来即期利率高估
	- 远期合约的价值将会上升，应买入
	- 如果债权的到期时长（maturity）大于投资期限，到期时长越长，持有期收益率（holding period return）越高
	- 使用 骑乘收益率曲线策略 将产生比 到期日匹配策略的收益
- 如果投资者认为远期利率对于未来即期利率低估
	- 和上面刚好相反

<br><br>

## 2\. 掉期利率曲线（swap rate curve）

<br><br>

掉期利率（swap rate）：

- 固定利率支付方（fixed-rate leg）的利率

### 即期利率（spot rate）vs 掉期利率（swap rate）

即期利率（spot rate）和掉期利率（swap rate）都可以用于基准利率（benchmark）

- 具体使用哪一个作为基准利率依照情况而定
- 批发银行（wholesale bank）常常利用掉期合约，转移风险，所以掉期利率常被用作为基准利率
- 零售银行（retail bank）较少使用掉期合约，即期利率常被作为基准利率

> - 批发银行的客户主要是商人银行（merchant bank）和其他的金融机构
> - 零售银行的客户主要是个人（individual）和小型企业（small business）

使用掉期利率 / 伦敦银行同业拆放利率（london inter bank offered rate (LIBOR)）作为基准利率的优点：

- 可以反映信用等级较高的（A1/A+）的私营信用主体（private entities）的违约风险（default risk）变化，大多数商业银行（commercial banks）的评级处在该水平
- 掉期合约是因为非标准化，场外交易（over-the-counter）的产品，所以不受政府影响，所以掉期利率更好的反映了市场供给与需求的变化，便于在不同国家之间进行资金成本的比较（comparable across different countries）
- 掉期期限的多样性，更易于绘制掉期利率曲线

利差（swap spread）

- 掉期利率利差（swap spread）= 掉期利率 - 相同期限的新发行（on-the-run）国债的到期收益率
- 利率利差（I-spread） = 某一个特定债券到期收益率 - 相同期限的掉期利率
	- 债券的收益率反映了时间价值（time value），信用风险（credit risk），流动性风险（liquidity risk），利率利差（I-spread）只反映信用风险，流动性风险
- 泰德利差（TED spread） = 伦敦银行同业拆放利率（LIBOR）- 短期国债（treasurary bill）的收益
	- 泰德利差反映的是银行系统（banking system）的风险

- 伦敦银行同业拆放利率 - 隔夜指数掉期利差（LIBOR - overnight indexed swap (OIS) spread）
	- 隔夜指数掉期合约的浮动利率是由隔夜拆借利率的几何平均值（geometic average of an overnight rate (or overnight index rate)）决定的
	- LIBOR - OIS利差反映了信用风险，体现了银行系统（banking system）整体状态（overall wellbeing）
- 零波动率利差（zero volatility spread / Z-spread）
	- 风险债券和相应国债利率的利差
	- 在即期利率的基础上加上零波动率利差，便是 风险债券 的折现率
	- 不适用于含权债权的估值

<br><br>

## 3\. 利率的期限结构的传统理论（traditional theories of the term structure of interest rates）

<br><br>

利率的期限结构的传统理论

1. 无偏预期理论（unbiased expectation theory）
2. 区间预期理论（local expectation theory）
3. 流动性偏好理论（liquidity preference theory）
4. 市场分割理论（segmented market theory）
5. 优先聚集地理论（preferred habitat theory）


**无偏预期理论（unbiased expectation thoery）**

- 远期合约是未来的即期利率的无偏预测（unbiased predictor）
	- 无偏预期的假设是投资者是风险中性的（risk neutral），不需要风险溢价（risk premium）
- 向上倾斜的即期利率曲线意味着未来的短期利率将上升

**区间预期理论（local expectation theory）**

- 在极短期的期限内，投资者不需要风险溢价（risk premium），近似与风险中性
- 较长的投资期限，投资者的对风险的态度可能会改变

**流动性偏好理论（liquidity preference theory）**

- 投资期限越长，投资者索取的流动性溢价（liquidity premium）越高
	- 向上倾斜的即期利率曲线可能只是因为流动性溢价，并不一定是未来的即期利率会上升
	- 向下倾斜的即期利率曲线暗示未来即期利率会快速下降

**市场分割理论（segmented market theory）**

- 每个投资者有各自的投资偏好（preferred maturity），而且恒定不变
- 所以不同的投资期限都有各自的需求和供给

**优先聚集地理论（preferred habitat theory）**

- 投资者存在各自的投资偏好，但是会根据不同投资收益率水平的差异做出调整
- 所以不同期限的利率水平并不是相互独立的

<br><br>

## 4\. 现代期限结构模型（modern term structure model）

<br><br>

现代期限结构模型（modern term structure model）可分为两类：

1. 均衡期限结构模型（equilibrium term structure models）
2. 无套利模型（arbitrage-free model）

### 均衡期限结构模型（equilibrium term structure models）

- 通过预测影响期限结构的经济基本面变量（fundamental economic variable）的变化，预测期限结构
- 可细分为两个模型：
	- 考克斯-英格索尔-罗斯模型（cox-ingersoll-ross model）
	- 瓦西塞克模型（vasicek model）

**考克斯-英格索尔-罗斯模型（cox-ingersoll-ross model）**

- 每个个体都在进行消费或者投资活动，消费决定了资金的需求，投资决定了资金的供给，供需关系决定了短期利率
- 长期利率是短期利率加上期限溢价（term premium）的结果
- 不同时刻的短期利率的变动（dr）可以用公式计算
- dr = a × ( b - r ) × dt + σ × √r × dz
	- a × ( b - r ) × dt 为趋势项（drift term），存在均值回归的特点，平均值为b，回归的速度为a
	- σ × √r × dz 为波动项（volatility term），**利率越大，波动率越大**

**瓦西塞克模型（vasicek model）**

- dr = a × ( b - r ) × dt + σ × dz
	- 趋势项（drift term）和考克斯-英格索尔-罗斯模型一样
	- σ × dz为波动项（volatility term），**波动性和利率无关**

### 无套利模型（arbitrage-free model）

**侯李模型（ho-lee model）**

- dr<sub>t</sub> = θ<sub>t</sub> × dt + σ × dz<sub>t</sub>
- 使用该模型之前，需先在市场上确定一组基础（reference set）债券
	- 基础债券的定价需正确
- 可由此推算出它们的折现率，进而确定候李模型的系数，θ<sub>t</sub>

<br><br>

## 5\. 收益率曲线因子模型（yield curve factor models）

<br><br>

收益率曲线因子模型（yield curve factor models）：

- 用于描述收益率曲线的变动

收益率曲线风险（yield curve risk）

- 由于收益率曲线发生变化而导致投资组合的价值变化的风险
- 本质是市场价格风险（market price risk）
- 变形风险（shaping risk）
	- 属于收益率曲线风险的一种类型
	- 收益率曲线发生非平行移动（non-parallel shift），比如短期利率上升的速度大于长期利率

收益率曲线因子模型（yield curve factor models）

- 收益率曲线可以分为三类
	- 斜率改变（steepness change），90%的收益率曲线变化来自于斜率改变
	- 平行移动（level change）
	- 曲度变化（curvature change）
- 将这些变化进行量化的描述就是收益率曲线因子模型

计量收益率曲线风险（meansure yield curve risk）

- 有效久期（effective duration）
	- 整体发生平行移动时，对债券价格的影响
- 关键利率久期（key rate duration）
	- 某个（局部）期限的即期利率发生变化，对债券价格的影响
- 对于平行移动，斜率改变，曲度变化的敏感度（sensitivity）
	- 具体的模型依靠观察者的主观定义

利率波动性的期限结构（term strucuture of interest rate volatilities）

- 计量的是收益率曲线风险
- 通常来说短期利率的波动性比长期利率的波动性大
	- 短期利率波动和货币政策有关（monetary policy）
	- 长期利率波动和实体经济（real economy）还有通货膨胀（inflation）有关

<br><br>

## 6\. 小结

一共提到了五种曲线

1. 即期利率曲线（spot curve）
2. 远期利率曲线（forward curve）
3. 平价利率曲线（par curve）
4. 收益率曲线（yield curve）
5. 掉期曲线（swap curve）
