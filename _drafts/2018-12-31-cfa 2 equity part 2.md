---
layout: post
title: CFA Level 2 权益 Part 2
categories: CFA2级笔记
---

## 目录

1. 绝对价值：现金流折现（discounted cash flow）
2. 现金流折现：股利折现模型（discounted dividend model）
3. 现金流折现：自由现金流价值（free cash flow valuation）
4. 相对价值：价格乘数（price multiple）

<br><br>

## 1\. 绝对估值法：现金流折现（discounted cash flow）

<br><br>

（续上一部分）

### c）预测资产负债表科目

因为利润表数据的预测在前，资产负债表的预测尽可能从利润表预测数据而进行预测，目的是为了保持财务报表的勾稽关系

<u>1\. 运营资金（working capital）</u>

- 存货（inventory）= 预测年度主营业务成本（COGS）/ 存货周转率（inventory turnover）
- 预测应收账款 = 应收账款周转天数（days sales outstanding）×（预测营业收入 / 365）

<u>2\. 财产、厂房和设备（property, plant and equipment）</u>

默认假设为主营业务的一定比率

应该将用于财产、厂房和设备的投资分为两类：

- 维持性资本支出（capital expenditure for maintenance）
- 增长性资本支出（capital expenditure for growth）

因为要考虑通货膨胀的问题，仅使用历史平均值是不足够的

### d）敏感性分析（sensitivity analysis）

当金融数据预测完成时，可以进行敏感性分析，观察公司在不同的商业环境下的净收入情况

### e）资本回报率（the return on invested capital）

资本投入（invested capital）= 运营资产（operating asset）- 运营负债（operating liabilities）

资本回报率（the return on invested capital）= 税后营业收益（net operating profit after tax (NOPAT)）/ 资本投入

- 税后营业收益 = EBIT × ( 1 - 税率）
- ROIC将权益和债务都算作资本，所以便于在不同公司之间做比较
- 有更高的资本回报率的公司运营更优

已动用资本回报率（return on capital employed）

- 使用的是EBIT而不是NOPAT，用于比较需上缴不同税率的公司

<br><br>

由波特五力模型分析公司的竞争地位（competitive position）

- 公司的定价能力（pricing power）取决于：
  - 替代商品的威胁性
  - 转化成本
- 公司的盈利能力取决于供应商的议价能力

分析师应理解公司的对冲（hedging）和垂直整合（vertical integration）策略

预测公司的剩余价值（terminal value）

- 相对价值法（relative valuation approach）
  - 价格乘数法（price multiples approach）：根据公司的市盈率数据等，配合合理的价格乘数估计
- 现金流折现法（discounted cash flow approach）
  - 两个重要自变量：现金流量 & 预期增长率

> 预测公司的剩余价值 和公司金融 part 3 的剩余价值的计算出现了重合

**两个基本的现金流折现模型**

1. 股利折现模型（discounted dividend model）
  - 适用于非控股股东
  - 主要收益来源是股利，以及出售时最终的股价（剩余价值）
2. 自由现金流价值（free cash flow valuation）
  - 适用于控股股东
  - 收益不仅包括股利，还来自于公司本身的盈利能力

<br><br>

##2\. 现金流折现：股利折现模型（discounted dividend model）
属于戈登股利增长模型（gordon growth model）的变体

<br><br>

基本假设

- 公司会持续派发股利，并存在一个持续稳定的增长率
- 增长率比要求回报率低

缺陷

- 对于增长率的估计依赖大
- 无法估计不派发股利的公司

公司的权益价值有两个部分

1. 公司永续权益现金流的现值（present value of a perpetual cash flow of equity）
2. 增长机会价值（present value of growth opportunities (PVGO)）
  - V<sub>0</sub> = E<sub>0</sub> / r + PVGO
  - E = 不再存在增长空间的收益水平（no-growth earning level (E<sub>0</sub> or E<sub>1</sub>)）
  - r = 权益要求回报率

**特殊情况**

优先股（preferred stock）的估值

- = D<sub>p</sub> / k<sub>p</sub>

二阶段（two-stage）股利折现模型（分为两种）

- 假设增长率A在某个时点切换为增长率B
- 假设增长率A常数速率直线下降，并在未来稳定为增长率B
  - 也称为股利折现H模型（H-model）

股利折现H模型（H-model）

- 增长率以常数速率直线下降，并在未来稳定在某个值
- 从图表上看，相当于计算一个长方形和三角形的面积
- V<sub>0</sub> = { [ D<sub>0</sub> × ( 1 + g<sub>L</sub> ) ] + [ D<sub>0</sub> × H ( g<sub>s</sub> - g<sub>L</sub> ) ] } / ( r - g<sub>L</sub>)
  - H = t / 2
  - [ D<sub>0</sub> × ( 1 + g<sub>L</sub> ) ] / ( r - g<sub>L</sub>) 相当于长方形 “面积”
  - [ D<sub>0</sub> × H ( g<sub>s</sub> - g<sub>L</sub> ) ] } / ( r - g<sub>L</sub>) 相当于三角形 “面积”

三阶段（three-stage）股利折现模型

- 和二阶段的原理类似，也分为两种假设


增长率的计算：

（两种计算方法本质是一样的）

可持续增长率（sustainable growth rate）

- = b × ROE
- b：1 - 股利支付率（dividend payout ratio）

PRAT模型

- g = 留存比率 × 边际利润 × 资产周转率 × 财务杠杆
- 边际利润（profit margin (P)）
- 留存比率（retention rate (R)）
- 资产周转率（asset turnover (A)）
- 财务杠杆（degree of financial leverage (T)）
- 相当于把ROE拆分成三分（杜邦分析）

杜邦分析

- 【三因子分解】ROE = （利润/营业收入）× （营业收入/总资产）× （总资产/权益）
- 【五因子分解】ROE = （利润/税前收益）×（税前收益/息税前收益）×（息税前收益/营业收入）× （营业收入/总资产）× （总资产/权益）

<br><br>

## 3\. 现金流折现：自由现金流价值（free cash flow valuation）

<br><br>

自由现金流分为两种：

- 权益自由现金流（free cash flow to equity）
- 公司自由现金流（free cash flow to firm）

**公司自由现金流（free cash flow to firm）**

- 全投资假设
  - 所以没有负债和利息
- = 除去现金支出后的现金收入（NOPAT + 非现金支出）- 运营资金投资 - 资本支出

**权益自由现金流（free cash flow to equity）**

- = 公司自由现金流 - 利息支出（考虑税盾的效果） + 新增贷款
- = 净收入 -（1 - 贷款比率（debt ratio）×（资本支出 - 折旧）-（1 - 贷款比率）× 运营资金

> ### 关于自由现金流的两个概念的解释

> 1\. 现金收入

> - 考虑的是现金性收入，所以当使用净利润进行计算时，应该考虑折旧，摊销，递延所得税等科目的影响

> 2\. 税后营业收益（net operating profit after tax (NOPAT)）

> - 全投资假设下的税后利润
> - 全投资假设：公司不存在借贷
> - = 息税前收益 ×（1 - 税率）

企业价值（enterprise value）

= 权益 +（负债 - 现金）

运营资金有两种理解方式：

- 【资产负债表】流动资产 - 流动负债
- 【营业性现金流（除去融资和投资）】流动资产（除去货币资金 & 约当资金）- 流动负债（除去含息负债）

特点

- 股利派发，股票回购，股票增发对于公司自由现金流 & 权益自由现金流没有影响
- 杠杆率变化对公司自由现金流无影响，对权益自由现金流有轻微影响

使用戈登增长模型计算权益价值

- = FCFE<sub>1</sub> / ( r - g ) = FCFE<sub>1</sub> × ( 1 + g ) / ( r - g )
- 可能存在一阶或者多阶，和前面的股利折现模型是一个原理
- 多阶计算存在剩余价值（terminal value），计算方法和前面介绍DCF时提到的方法一样，分为现金流折现法和相对价值法

敏感性分析

- 因为自由现金流模型对自变量依赖较大，所以需要对这些自变量进行敏感性分析/情景分析
- 营业收入的增长率


## 4\. 相对估值法：价格乘数（price multiple）

<br><br>

> 实际上，公司分析时，更常见的价格乘数

> - 企业价值/营业收入
- 企业价值/税息折旧及摊销前利润（EBITDA）
- 企业价值/息税前利润
- 企业价值/净利润
- 企业价值/营业面积
- 企业价值/点击量


价格乘数的作用：

- 对某一公司进行估值
  - 寻找一系列可比公司（comparable companies）
  - 计算他们的价格乘数，并取平均值
  - 理论上说，这个平均值就是被研究公司应该有的价格乘数
  - 将这个价格乘数，和公司的财务数据结合，逆推出一个理论的股票价格
  - 将理论股票价格和实际股票价格进行对比
  - 通过对比估测公司股价是否被高估/低估


在计算平均值时，使用的是调和平均数（harmonic mean）

- 调和平均数 = 1 / Σ (W<sub>i</sub>/ X<sub>i</sub>)
- 即：取各公司的乘数的倒数，以股价为权重加总，再将结果取倒数
- 能够降低异常值（outlier）对于平均值的影响

### 基本比率

** <u>1\. 市盈率（EPS） </u>**

将每股收益标准化（normalizing EPS），有两种方法

1. 历史平均市盈率
  - 没有考虑公司的规模的因素
2. 平均ROE
  - ROE × 每股账面价值 = EPS
  - 比第一个方法更好

判断股市是否被低估/高估的两个模型：

1\. 联邦储备模型（fed model）

- 联邦储备模型利率 = 标普500收益率（S&P earning yield）/  10年期国债收益率
  - 收益率（earning yield）= 每股收益/每股市值
  - 联邦储备模型利率 > 1，股市整体被低估

2\. 亚德尼模型（yardeni model）

- E<sub>1</sub> / P<sub>0</sub> = y<sub>B</sub> - d × LTEG
  - y<sub>B</sub> = 穆迪A级（Moody's A-rated）公司债券收益率
  - LTEG = long term earning growth = 标普500未来5年的收益增长率一致预期（consensus）
  - 戈登股利增长模型的变体： E<sub>1</sub> / P<sub>0</sub> = r - g
  - 其中：r =  y<sub>B</sub>，g = LTEG

如果E<sub>1</sub> / P<sub>0</sub> >  y<sub>B</sub> - d × LTEG，市场被低估

** <u>2\. 市盈率（P/E）</u>**

市盈率与增长比率（P/E to growth ratio (PEG)）

- = P/E ratio / g

真实市盈率（justified P/E）

- 【优点】计量直观，反映大约需要多少年回收投资资本
- 【缺点】不适合收入低而未来发展前景高的创业公司，或者利润为负的公司
- 动态市盈率（leading P/E）= P<sub>0</sub> / E<sub>1</sub> = ( 1 -  b ) / ( r - g )
  - b：股利支付率
  - 分析师一般使用动态市盈率
- 静态市盈率（trailing P/E）= P<sub>0</sub> / E<sub>0</sub> = ( 1 - b ) × ( 1 + g ) / ( r - g )

推导过程

P<sub>0</sub> / E<sub>1</sub> = ( D<sub>1</sub> /  E<sub>1</sub> ) / ( r - g ) = ( 1 -  b ) / ( r - g )
- 戈登增长模型：P<sub>0</sub> = D<sub>1</sub> / ( r - g )
- D/E = 股利支付率 = 1 - 收益留存率 = ( 1 - b )

** <u>3\. 市净率（P/B）</u>**

**真实市净率（justified P/B）**

- 【优点】适用于估算银行，重工业
- 【缺点】账面价值不能反映市场价值
- 动态市净率（leading P/B）= P<sub>0</sub> / B<sub>1</sub> = ( 1 -  b ) × ROE / ( r - g )
- 静态市净率（trailing P/B）= P<sub>0</sub> / B<sub>0</sub> = ( 1 -  b ) × ROE × ( 1 + g ) / ( r - g )
- 分析师一般使用静态市净率

** <u>4\. 市销率（P/S）</u>**

**真实市销率（justified P/S）**

- 【优点】适用于估值濒临破产的公司，当市盈率，甚至市净率为负数时
- 【缺点】可以通过提前确认营业收入的方式操纵市销率
- 动态市净率（leading P/S）= P<sub>0</sub> / S<sub>1</sub> = ( E<sub>0</sub> -  S<sub>0</sub> ) × ( 1 - b) / ( r - g )
- 静态市净率（trailing P/S）= P<sub>0</sub> / S<sub>0</sub> = ( E<sub>0</sub> -  S<sub>0</sub> ) × ( 1 - b) × ( 1 + g ) / ( r - g )

** <u>5\. 市现率（P/CF）</u>**

- 【优点】现金流不易被操纵
- 【缺点】波动性高

现金流的计算有以下四种方式

1. 利润加上非现金支出（earning-plus-noncash-charges）
  - = 净收益 + 折旧 + 摊销
  - 【缺陷】没有考虑非现金性营业收入和运营资金的变化
2. 调整后营业性现金流（adjusted CFO）
  - = 营业性现金流 + [（净现金利息支出）×（1 - 税率）]
  - 【缺陷】没有考虑投资性和融资性活动
3. 权益自由现金流
4. EBITDA
  - EBITDA更多用于计算公司的企业价值（权益+ 债权），作为企业价值/EBITDA比率，而不是像先前的几个比率计算的是权益价值

- 【EBITDA优点】可用于对比有不同程度的财务杠杆的公司
- 【EBITDA缺点】当运营资金在增加时，EBITDA会高估企业价值

** <u>6\. 股息率（dividend yield）</u>**

- 动态股息率 = 预测未来四个季度的股利 / 每股市值
- 静态股息率 = 最近四个季度的股利 / 每股市值

真实股息率（justified dividend yield）

静态股息率 = D<sub>0</sub> / P<sub>0</sub> = ( r -g ) / ( 1 + g )

<br><br>

**价值动量指标（momentum valuation indicator）**

超出预期利润（unexpected earning）

- 公司报告的实际利润 - 过去市场的一致预期

**相对强弱指标（relative strength (RSTR) indicator）**

分为两类

- 和公司的历史比较（时间序列模型）
- 和同行业进行比较

比较的对象

- 权益回报率
