---
layout: post
title: CFA Level 2 投资组合 Part 1
categories: CFA2级笔记
---
## 目录

1. 经典理论模型：资本资产定价模型（Capital Market Pricing Model）
2. 经典理论模型第一类修改：套利定价理论（APT Arbitrage Pricing Theory）
3. 经典理论模型第二类修改：多因子模型（Multifactor Models）
4. 主动投资的风险和收益（Active Risk and Return）

<br><br>

## 1\. 经典理论模型：资本资产定价模型（Capital Market Pricing Model）

* **E (R<sub>i</sub>) = R<sub>f</sub> + β (E(R<sub>M</sub>) - R<sub>f</sub>)**
* 是单因子模型，只和系统性风险有关

> 资本资产定价模型假设：

> - 所有投资者都是马科维茨（Markowitz）投资者，寻找效用最大化
- 市场是完全有效的，所有投资者都是价格承受者
- 所有投资者投资期限相同而且只投一期
- 资本市场是无摩擦市场，没有交易费用
- 资产无限可分
- 投资者有相同期望

<br><br>

## 2\. 经典理论模型第一类修改：套利定价理论（APT Arbitrage Pricing Theory）

**优点**
相比资本资产定价模型，前提假设少，而且符合实际

**缺点**
不知道具体那些（GDP，失业率等）因子应该被考虑，因子的数量也未知

**假设**

- 资产收益率是受多个因数影响（multiple factor model）
- 资产相关的风险（Asset-specific）可以被分散化
- 不存在套利机会

公式： **E (R<sub>P</sub>) = R<sub>F</sub> + β <sub>P,1</sub> (λ<sub>1</sub>) +  β <sub>P,2</sub> (λ<sub>2</sub>) + ... + β <sub>P,k</sub> (λ<sub>k</sub>)**

纯因子模型
只有一个β = 1 ，其他β = 0的投资组合

<br><br>

## 3\. 经典理论模型第二类修改：多因子模型（Multifactor Models）
1. 宏观经济因子模型（Macroeconomic factor models）
1. 基本面因子模型（Fundamental factor models）
1. 统计因子模型（Statistical factor model）

<br><br>

### 宏观经济因子模型（Macroeconomic factor models）

**公式：R<sub>i</sub> = E(R<sub>i</sub>) + b<sub>i1</sub>F<sub>1</sub> + b<sub>i2</sub>F<sub>2</sub> + ... + b<sub>ik</sub>F<sub>k</sub> + ε**

* 截距（intercept）：资产i的期望收益率（expected return of asset i）
* F: 风险定价因子，超出预期的宏观经济变量（Priced risk factors, surprise in the macroeconomic variables）
* b: 因子敏感度（斜率），类似于资本资产定价模型中的β（Factor sensitivities, similar to betas in the market model）
* E(R<sub>i</sub>)  可以通过资本资产定价模型或者套利定价理论算出

**特点：**

  1. 这是一个回归模型
  1. 套利定价理论计算的是期望收益率，宏观经济因子模型是（预测的）实际收益率

<br><br>

### 基本面因子模型（Fundamental factor models）
**R<sub>i</sub> = a<sub>i</sub> + b<sub>i1</sub>F<sub>1</sub> + b<sub>i2</sub>F<sub>2</sub> + ... + b<sub>ik</sub>F<sub>k</sub> + e<sub>i</sub>**

* F: 因子收益率，每个因子相关的收益率，由多元回归计算而得（factor returns, rates of return associated with each factor, estimated using multiple regression）
* b: 标准化敏感度（类似于z统计量），并不是斜率（standardized sensitivities (similar to z-statistics), not regression slope estimates）

> 和宏观经济因子模型不同之处在于：
>
> * b不是斜率而是标准化敏感度；不是回归计算而得，而是标准化计算而得
> * F不是变量本身而是因子产生的收益率；不是直接套用数据，而是通过回归计算获得的

**套利定价模型和多因子模型的对比**

- 特点
  - 套利定价模型：横截面型的定价平衡点模型（cross-sectional equilibrium pricing model），用于解释资产期望收益的波动
  - 时间序列回归模型（time-series regression），用于解释长期以来某一特定资产的收益的波动
- 假设
  - 无套利机会
  - 依情况而定，观察对象不同，假设也可能会发生变化
- 纵截距
  - 无风险利率
  - 由无套利定价模型算出的预期收益率

<br><br>

### 多因子模型的应用（Multifactor model applications）
- 收益归因（Return attribution）
- 风险归因（Risk attribution）
- 投资组合的建立，例如因子投资组合（Portfolio construction (e.g. factor portfolio)）
- 策略性投资决策（Strategic portfolio decision (Comparative advantage and disadvantage in bearing risk))

<br><br>

## 4\. 主动投资的风险和收益（Active Risk and Return）
1. 增值（Value added）
2. 基本法则（fundamental law）

<br><br>

### 增值（Value added）
> 增值 = 主动收益（Active Return）

**主动收益（追踪误差）**，投资组合和基准的偏差（Active Return (tracking error)）

- 公式 R<sub>A</sub> = R<sub>P</sub> - R<sub>B</sub>

**主动风险（追踪风险）**，主动收益的标准差（Active risk(tracking risk)）

- 公式 s(R<sub>P</sub> - R<sub>B</sub>)= √(Σ(R<sub>Pi</sub> - R<sub>Bi</sub>)<sup>2</sup>/(n-1))
- 风险归因：主动收益的方差 = 因子（宏观）风险 + 证券自身风险（active risk squared = active factor risk + active specific risk）

风险调整后增值（Risk-adjusted calculation of value added），即alpha （α）
α<sub>A</sub> = R <sub>P</sub> - β<sub>P</sub> R<sub>B</sub>

产生正增值：收益率高的资产权重大，收益率低的资产权重小
R<sub>A</sub> = R<sub>P</sub> - R<sub>B</sub> = ΣW<sub>P,i</sub> R<sub>i</sub> - ΣW<sub>B,i</sub> R<sub>i</sub> = ΣΔW<sub>i</sub> R<sub>Ai</sub>
- ΔW<sub>i</sub> = W<sub>P,i</sub> - W<sub>P,i</sub>
- R<sub>A,i</sub> = R<sub>i</sub> - R<sub>B</sub>

增值（value added）= 来自资产分配的增值（value added from asset allocation） + 来自证券选择的增值（value added from security selection）
> 业绩归因

**（事前或事后）夏普比率**（Sharpe ratio:absolute expected (ex ante) or realized (ex post) reward-to-risk measure）
SP<sub>P</sub> = （R<sub>P</sub> - R<sub>f</sub>）/ σ<sub>P</sub>
> 承担单位总风险获得的额外的风险溢价

- 夏普比率不受杠杆率（leverage）影响
- 夏普比率受风险资产的权重（aggresiveness of active weight）的改变影响

**事后信息比率（ex-post information ratio）**
IR = （R<sub>P</sub> - R<sub>B</sub>）/ s(R<sub>P</sub> - R<sub>B</sub>)

- 信息比率受杠杆率（leverage）影响
- 夏普比率不受风险资产的权重（aggresiveness of active weight）的改变影响
- 平均主动收益和平均主动风险的比例
- 表示投资经理收集，处理信息的能力高

（无限制的，通过自动投资和被动投资的组合的混合）**调整主动风险**
SR<sub>P</sub><sup>2</sup> = SR<sub>B</sub><sup>2</sup> + IR<sup>2</sup>
- 调整主动风险的最优化（optimal level）： σ<sub>A</sub> = (IR / SR<sub>B</sub>) σ<sub>B</sub>

### 基本法则（fundamental law）
**事前（Ex ante）**

期望主动收益（追踪误差）
= 信息比率 × 期望主动风险（追踪风险）
= 信息系数 × 转化系数 × 宽度 × 期望主动风险（追踪风险）

（E(R<sub>A</sub>)
= Information Ratio × σ<sub>A</sub>
= Information Coefficient × Transfer Coefficient × √Breadth × σ<sub>A</sub>）

- 信息系数（Information Coefficient）：预测的主动收益和实际主动收益的相关系数
- 转化系数（Transfer Coefficient）：预测到的主动收益和因此调整的权重的相关系数（预测到了，但是否实际上完全付出了行动？）
- 宽度（Breadth）：一年内做出的独立决策的次数

> **转化系数不一定为1：**可能因为投资政策的限制，持股比例，限定的债券购买（BBB以下不能购买），所以预测到的主动收益不一定能够付出行动
>
> 信息系数，投资水平
> 宽度，努力程度

**事后（Ex post）**

期望主动收益（追踪误差） = 已知信息系数 × 转化系数 × 宽度 × 期望主动风险（追踪风险）

（E(R<sub>A</sub> | IC<sub>R</sub>) = Realized Information Coefficient × Transfer Coefficient × √Breadth × σ<sub>A</sub>）

> 和事前的区别是信息系数（Information Coefficient）是已知的了，所以是已知信息系数（Realized Information Coefficient）

实际收益率 = 期望主动收益（追踪误差） + 噪音
R<sub>A</sub> = E(R<sub>A</sub> | IC<sub>R</sub>) + Noise

（有限制的，通过自动投资和被动投资的组合的混合）**调整主动风险**
SR<sub>P</sub><sup>2</sup> = SR<sub>B</sub><sup>2</sup> + TC × (IR ')<sup>2</sup>
- 调整主动风险的最优化（optimal level）： σ<sub>A</sub> = (TC × IR ' / SR<sub>B</sub>) σ<sub>B</sub>

> 可以对比之前无限制的区别：多了一个转化系数

基本法则的应用

- 海外投资配置
- 债券的投资时机

基本法则的局限

- 事前的信息系数难估计
- 独立决策的次数的不确定性
