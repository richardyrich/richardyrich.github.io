---
layout: post
title: CFA Level 2 权益 Part 3
categories: CFA 
---

## 目录

1. 绝对价值：剩余收益价值（residual income valuation）
2. 非上市公司价值（private company valuation）

<br><br>

## 1\. 剩余收益价值（residual income valuation）

<br><br>

 剩余收益（residual income），又称为经济收益（economic profit）
 
 两个关键概念
 
-  剩余收益（residual income） 
  - 在公司金融中涉及了，所以不赘述了
-  经济增加值（economic value added）
  -  相当于公司金融的经济收益（economic profit）
- 市场增加值（market value added）
  - 有两种理解方式

市场增加值

1. 用公司金融部分的角度来理解，市场增加值为公司创造的价值
  - 所以这里的收益和资本投入都是相对于股权人 + 债权人而言的
  - = Σ [经济增加值/（1 + WACC）<sup>t</sup>] + 资本（股 + 债）投入
2. 也可以从对于股东的角度来理解，市场增加值为股东创造价值
  - 这里的资本仅仅使用股东资本，依然使用账面价值是因为有类似于持有期回报率的意思
  - = Σ [保留盈余/（1 - 股东要求回报率）<sup>t</sup>] + 股东资本投入


> ### 和公司金融部分的联系
> 
> **1\. 在公司金融 part 2 中将这两个名词命名了两个不同的估值模型，要注意区别**

> - 在公司金融中，剩余收益特指股东的收益，而经济收益泛指公司收益
> - 在权益part 3 这里，剩余收益和经济收益都特指股东的收益
> - 无论定义如何，基本原理都是：收益 - 机会成本

> **2\. 公司金融中出现的公式**

> a. 剩余收益（residual income） 
> - = 股东净收益（net income<sub>t</sub>） - 股东要求权益收益率（r<sub>e</sub>）× 股东投入初始金额（B<sub>t-1</sub>）

> b. 经济增加值 / 经济收益（economic value added / economic profit）

> - = 税后营业收益（net operating profit after tax (NOPAT)）-  加权平均资本成本额（dollar WACC）
> - = 息税前利润（EBIT） × （ 1 - 税率） - 加权平均资本成本（WACC） × 资本额（capital）
> - 资本额 = 权益投资 + 债务投资

> c. 市场增加值（market value added）：

> - 将每一期的经济增加值 / 经济收益折现并进行加总，相当于计算净现值（NPV），折现率为WACC
> - 市场增加值（market value added）= 净现值（NPV）= Σ economic profit<sub>t</sub> / (1 + WACC)<sup>t</sup>
> - 公司价值（V<sub>firm</sub>） = 市场增加值（market value added） + 投资额（investment）

<br><br>

### 剩余收益的“戈登增长模型”（以及与市净率的关系）

**1\. 【单期】两种表示方法（两个公式实际是一样的）**

- （增长模型）V<sub>0</sub> = B<sub>0</sub> + B<sub>0</sub> × ( ROE - r<sub>e</sub> ) / ( r<sub>e</sub> - g ) 

- （市净率）P<sub>0</sub> / B<sub>0</sub> = 1 + ( ROE - r<sub>e</sub> ) / ( r<sub>e</sub> - g )

分析

- 按照公式来理解：如果ROE大于要求回报，获得更多的剩余收益
- 不同于股利增长模型 & 权益自由现金流增长模型，计算方式是将现金流折现，剩余价值的增长模型是一个逐期叠加的模型

> 推导过程

> P<sub>0</sub> = V<sub>0</sub>

> - 【“戈登增长模型”】V<sub>0</sub> = B<sub>0</sub> + residual income / ( r<sub>e</sub> - g )
> - 【稍作变形】V<sub>0</sub> = B<sub>0</sub> + B<sub>0</sub> × ( ROE - r<sub>e</sub> ) / ( r<sub>e</sub> - g ) 
> - 【同时除以B<sub>0</sub>】P<sub>0</sub> / B<sub>0</sub> = 1 + ( ROE - r<sub>e</sub> ) / ( r<sub>e</sub> - g )

> 注意区别真实静态市净率的公式

> - P<sub>0</sub> / B<sub>0</sub> = ( 1 - b ) × ROE × ( 1 + g ) / ( r - g )

隐含增长率

- 将上述公式进行变形： g = r - [ B<sub>0</sub> × ( ROE - r ) / ( V<sub>0</sub> - B<sub>0</sub> ) ] 

<br><br>

**2\. 【多期（增长模型）】是三个部分的加总**

- 是单期模型的简单修改
- 账面价值 + 中期剩余收益的现值 + 长期剩余收益的现值

剩余价值的现值：

residual income<sub>T</sub> / ( 1 + r - ω )

剩余收益的折现并加总

公式：residual income<sub>T</sub> / ( 1 + r - ω )

- ω：持续因子（persistence factor）
  - 取值范围：0 < ω < 1
  - 当ω = 1 时，相当于永续，无限期
  - 当ω = 0 时，相当于剩余价值只持续了一期

持续因子的分析

- 更高的持续因子
  - 常伴随着更低的股利支付率
  - 存在行业特性
- 更低的持续因子
  - ROE过高
  - 公司的收入依赖于不可持续项目（nonrecurring items）
  - 报表存在过多应计项目（accrual）

多期的剩余收益的变化有四种常用假设

1. 剩余收入将持续
  - ω = 1
2. 立即下降为零
  - ω = 0
3. 等于行业平均值
4. ROE将逐渐等于权益融资成本（=权益要求回报率）
  - ω 介于0和1之间，每年的剩余收益都是上一年的 （1 - ω）倍
  - 相当于一个等比数列的加总

**剩余收益价值模型的优点&缺点**

- 【优点】不存在剩余价值（terminal value），所以可以作为现金流折现模型的替代
- 【优点】可用于计算现金流为负，或者不派发股利的公司
- 【缺点】相关的财务数据可以被操纵，所以需要对其进行调整

财务报表的应计原则（accrual）导致公司的资产价值会偏移市场价值，所以需要额外注意至少以下六种情况

1. 经营租赁
2. 特殊目的实体
3. 储备项（reserve）和计提拨备项（allowances）
4. LIFO vs FIFO
5. 养老金资产或负债
6. 递延所得税负债

<br><br>

## 2\. 非上市公司价值（private company valuation）

<br><br>

估值的三种方法

1. 收入类（income-based）
2. 市场类（market-based）
3. 资产类（asset-based）

私有公司可能存在为了减税而进行的支出

购入私有公司的动机可以分为两类

1. 战略性购买（strategic purchase）
  - 目的是为了和现有业务形成协同效应（synergy）
2. 金融性购买（financial purchase）
  - 为了获得额外的现金流

进行自由现金流计算时，更倾向使用公司自由现金流，因为更加稳定

### 收入类（income-based）估值

1. 剩余收益（residual income）
2. 超额盈余（excess earning）
  - 在超额盈余的算法中，公司自由现金流替代了标准化收益（normalized earning），自由现金流的增长率替代了剩余收益的增长率

估算非上市公司的折现率

1. 规模溢价
  - 规模小所以溢价高
2. 债券融资成本
  - 非上市公司贷款的渠道更少，所以公司的WACC更接近于权益融资成本
3. 收购方的估值
  - 收购方往往使用的是自身的折现率（WACC更高），所以导致高估了被收购公司的价格
4. 预测风险
  - 非上市公司信息更少
5. 生命周期
  - 公司越新越难估值

折现率的三个模型

1. CAPM
2. 扩张后（expanded）CAPM
  - 对CAPM进行修改，考虑到非上市公司带来的规模溢价等问题
3. 累加法（build-up method）

### 市场类（market-based）估值

使用价格乘数进行估值

1. 上市公司参照法（guideline public company method）
  - 需要考虑非上市公司的控股溢价（control premium）
2. 交易参照法（guideline transaction method）
  - 假如被参照的公司可比性高，所以调整程度不大
3. 过往交易法（prior transaction method）
  - 使用被收购公司的历史股份交易价格
  - 但是历史数据可能不具有代表性，而且可能没有控股溢价

因为非上市公司存在流动性风险等问题，所以相对于上市公司的估值来说，非上市公司的估值需要额外注意

市场乘数

- 大型公司：EBIT/EBITDA 乘数
  - EBIT除去了财务杠杆的影响，EBITDA排除了重大非现金支出的的影响
- 小型公司：净收入乘数

### 资产类（asset-based）估值

用于估值特殊行业和濒临破产公司

依然要考虑是否存在控股 & 市场性（marketability）（相当于“流动性”）的溢价

- 非控股折价（discount of lack of control）
  - = 1 - [ 1 /（ 1 + 控股溢价 （control premium））]
- 市场性折价
  - = 1 - [ 1 /（ 1 + 市场型溢价 （marketability premium））]