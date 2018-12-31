---
layout: post
title: CFA Level 2 公司金融 Part 1
categories: CFA 
---

## 目录
1. 资本预算（capital budgeting）
2. 公司市场价值的估值方法（market value evaluation metiod）
3. 估值方法 1：经济收入（economic income）

<br><br>

### 1\. 资本预算（capital budgeting）

<br><br>

**资本预算（capital budgeting）**

- 考虑增量现金流（incremental cash flow）
- 不考虑沉没成本（sunk cost）
- 考虑外部性（externality）
  - 负外部性（negative externality）
  - 正外部性（positive externality）
- 时间（timing）
- 计算取税后的数字（after tax basis）

**资本预算的分类（categories of budgeting project）**

- 替代项目（replacement project）
  - 为了公司的继续经营（maintain the business）而进行的替换
  - 为了降低公司的成本（cost reduction purpose）而进行的替换
- 扩张项目（expansion project）
  - 原有项目（existing product）的扩张
  - 新项目（new project）的扩张
- 政府强制实施的项目（mandatory investment）
  - 比如政府要求的，法律要求的
- 其他

<br><br>

### a）扩张项目（expansion project）vs 替代项目（replacement project）

<br><br>

**扩张项目（expansion project）**

- 固定资产投资（fixed capital investment）
- 净运营资金投资（net working capital investment）
- 分为三个阶段
  - 初始支出（initial outlay）
  - 运营阶段（operating stage）
  - 终止阶段（terminating stage）

  > 可以想象成一个债券，初始支付一个费用，并在后来不断地接收息票，最后收回本金（虽然只有一部分）


**1\. 初始支出（initial outlay）**

- 初始支出 = -（固定资产投入 + 净运营资金投资）
- 净运营资金投资 = △Asset <sub>non-cash current</sub> - △Liability<sub>non-debt current</sub>
  - 一般来说不考虑现金和短期债务的影响

**2\. 运营阶段（operating stage）**

- 运营现金流（operating cash flow） = （运营收入（sales） - 成本（cost） - 折旧（depreciation））×（1 - 税率（tax rate））+ 折旧（depreciation）
  - 上面的公式化简后
  （收入-成本）×（1-税率）+ 折旧 × 税率
  - 因为折旧会产生税收利益，所以才会出现在公式里

**3\. 终止阶段（terminating stage）**

- 在终止时期的运营现金流（operating cash flow at terminating stage）
- 运营资金的收益（return of working capital）
- 固定资产的售出（sale of fixed asset）
- 终止阶段的经营现金流的计算其实就是运营的最后一期，所以和运营阶段的现金流计算是一样的
- 终止阶段的经营现金流 = 净运营资金投入 + 固定资产的售出价格 （Sal<sub>T</sub>）- （固定资产的售出价格（Sal<sub>T</sub>） - 固定资产的账面价值（B<sub>T</sub>））× 税率

**替代项目（replacement project）**

- 和扩张项目一样分为三个阶段
  - 初始支出（initial outlay）
  - 运营阶段（operating stage）
  - 终止阶段（terminating stage）
    > 与扩张项目（expansion project）项目不同的是，初始存在一个出售旧设备的收入

**1\. 初始支出（initial outlay）**

- 初始支出 = -（固定资产投入 + 净运营资金投资）+ [旧设备售出价格（Sal<sub>0old</sub>） - （旧设备售出价格（Sal<sub>0old</sub>）- 旧设备账面价值（B<sub>0old</sub>）× 税率（tax）]
- 固定资产投入（fixed capital investment）
- 运营资金投入（working capital investment）
- 旧设备的卖出（sale of old fix asset）

**2\. 运营阶段（operating stage）**

- 运营现金流（operating cash flow）= （更换后的收入（△S） - 更换后的成本（△C））×（1 - 税率）+ 更换后的折旧（△D） × 税率
  - 假设新旧设备的使用年限是一样的

**3\. 终止阶段（terminating stage）**

- 终值净现金流（terminating net operating cash flow）  = 净运营资金投入（net working capital investment） + [ 新设备售价（Sal<sub>Tnew</sub>） - （新设备售价（Sal<sub>Tnew</sub>） - 新设备账面价值（B<sub>Tnew</sub>）× 税率 ] -  [旧设备售价（Sal<sub>Told</sub>）-（旧设备售价（Sal<sub>Told</sub>） - 旧设备售价账面价值（B<sub>Told</sub>））× 税率]
- 运营现金流（operating cash flow）
- 运营资金（working capital）
- 固定资产的售出（sale of fixed asset）

### 小结

- 扩张项目（expansion project）可以看做是初始为无的替代项目（replacement project），所以替代项目和扩张项目本质是一样的
- 替代项目存在出售旧有设备，所以存在多一笔现金流，减少了初始支出（reduce the initial outlay）

<br><br>

### b）加速折旧法（modified accelerated cost recovery system (MACRS)）

<br><br>

美国国内税收法（US internal revenue code）使用加速折旧法（modified accelerated cost recovery system (MACRS)）进行对折旧的所得税减免计算（tax deduction with depreciation）
- 应折旧额（depreciable basis） = 购入价格（purchase price） + 运输/处理和安装费用（shipping/handling and installation costs）

### c）通货膨胀（inflation）

<br><br>

- 使用正确的折现率
	- 真实现金流（real cash flow）应使用真实折现率（real discount rate）折现
	- 名义现金流（nominal cash flow）应使用名义折现率（nominal discount rate）折现
	- 计算的出来的NPV相等
- 如果通货膨胀率超出预期
	- 收益会低于预期
	- 所得税增加，因为折现税盾（depreciation tax shelter）的效果将低于预期
	- 债权人（bondholder）获得的固定收益（fixed payment）价值降低
- 通货膨胀对于公司的影响是弊大于利，因为涨价困难

<br><br>

### d）互斥项目之间的选择

<br><br>

CFA Level 1 中提到，两个互斥项目，选择NPV高的一项，前提条件是项目的期限是一样长
如果不一样则使用以下两种方法进行评估：

- 最小公倍数（least common multiple of lives approach）
	- 取两个项目的最小公倍数，并且将两个项目重复进行，直到达到公倍数时长（lives divide equally into the chosen time horizon）
- 年金法（equivalent annual annuity (EAA) approach）
	- 将两个项目转化成两个每年派发固定数额的年金，年金的现值（NPV）等于项目各自的现值



### e）资本限额（capital rationing）

<br><br>

1. 强制资本限额（hard capital rationing）
  - 上限不可被提高（cannot be increased）
2. 弹性资本限额（soft capital rationing）
  - 上限可以提高（allowed to increase），前提是可以合理的为股东创造价值（create shareholder value）

### f）风险分析（risk analysis）

<br><br>

风险分析（risk analysis）

1. 独立分析（stand-alone method）
2. 市场风险分析（market risk method）

**独立分析（stand-alone method）**

- **敏感性分析（sensitivity analysis）：** 修改某一个因子
- **情景分析（scenario analysis）：** 同时改变数个因素
- **模拟分析（simulation analysis）：** 又名“蒙特卡罗模拟” ，从一定范围内按一定方法随机选择定义因素的量

**市场风险分析（market risk method）**
> 相比独立分析（stand-alone method），市场风险分析（market risk method）是从整体进行分析

<br><br>

### g）项目分析(project evaluation)

<br><br>

**项目折现率vs公司折现率**

- 项目折现率
	- 常用资本资产定价模型（capital asset pricing model (CAPM)）来计算项目的最低收益率
	- R<sub>project</sub> = R<sub>f</sub> + β<sub>project</sub>[ E(R<sub>M</sub>) - R<sub>f</sub> ]
- 公司折现率
	- 常使用加权平均资本成本（weighted average cost of capital (WACC)）来计算
- 不能简单的通过将公司的所有项目的折现率进行加权平均算出公司的总体的折现率，因为项目之间可能存在可能的相关性，增加或者降低公司的风险。在这种情况下，如果坚持使用WACC来计算项目的NPV：
	- project's risk > comapany's risk → overestimate the NPV
	- project's risk < comapany's risk → underestimate the NPV

**实质选择权（real option）**

- 将现有可选项目的估值进行调整（alter the value of capital budgeting），依据的是该项目对未来项目可能产生的外部性
- 像金融期权（financial options）一样，实质选择权的价值和未来项目有关（contingent on future events）

**实质选择权（real option）一共有四类**

- 时机选择权（timing option）
	- 使得公司能够递延投资（delay investing）
- 规模选择权（sizing option）
	- 放弃选择权（abandonment option）
	能够让公司终止项目，如果继续带来的损失大于终止
	- 扩张选择权（expansion option）
	让公司进行额外投资，如果项目能够带来更多收益
- 弹性选择权（flexibility option）
	- **定价选择权（price-setting option）**
	可以直接因为涨价带来额外收益，而不需改变生产量
	- **生产选择权（production flexibility option）**
	可以从加班（working overtime）和增加班次（additional shift）来增加收益
- 基本选择权（fundamental option）
	- 价值取决于项目本身，类似金融期权（financial options）

**实质选择权的四种估值方法**

1. 假设选择权不存在的情况下估值项目的NPV
	如果项目本身的NPV已经 > 0，那么加上实质选择权的价值会 > 0， 所以应该进行该项目
2. 在不考虑选择权下，计算项目的NPV，在其基础再加上实质选择权的估值
  Overall NPV = project NPV ( based on DCF ) + option value - option cost
3. 使用决策树（decision tree）
4. 使用选择权定价模型（option pricing model）

### h）资本预算的常见错误（common pitfalls）

<br><br>

1. 没有考虑经济环境（economic response）
2. 过度依赖模式化（evaluation templates）的分析方法
3. 对于喜好项目（pet projects）的乐观估计
4. 因为出于短期的每股收益，净收入，股本收益率（EPS, NI, ROE）的考虑，而导致长期项目被迫放弃
5. 依赖内部收益率（IRR）做决定，因为IRR可能出现无解或者多个解的情况
6. 对未来现金流的估计偏差（poor cash flow estimation）
7. 错估经常花费（estimating overhead costs），某些花费可能由多个项目共用，所以难以判定
8. 使用错误的风险调整后折现率（risk-adjusted discount rate）
9. 办公室政治（politics）对于资本预算的影响
10. 没有考虑到别的投资选项（failure to generate alternative investment ideas）
11. 没有正确处理好沉没成本（sunk cost，不应该考虑）和机会成本（opportunity cost，应该考虑）

<br><br>

## 2\. 公司市场价值的估值方法（market value evaluation metiod）

1. 税后现金流（after-tax cash flow）
2. 经济收益（economic profit）
3. 剩余收益（residual income）
4. 索取权价值（claims valuation）

<br><br>

## 3\. 估值方法 1：税后现金流（after-tax cash flow）

<br><br>

经济收入（economic income）vs会计收入（accounting income）

- 经济收入（economic income）：
	- 税后现金流（after-tax cash flow） + 项目的经济折旧（economic depreciation，市场价值变动）
	- 经济收入 = 税后现金流 - 经济折旧（期初市场价值 - 期末市场价值） = CF - ( MV<sub>t-1</sub> - MV<sub>t</sub> ) = CF - △MV
	- 经济折旧 = 期初市场价值 - 期末市场价值
- 会计收入（accounting income）：
	- CFA会计部分的内容，在公司金融部分不考


**如何理解经济折旧（economic depreciation）**

| -            | 0              | 1              | 2              |
|--------------|----------------|----------------|----------------|
| Cash flow    |        -        | CF<sub>1</sub> | CF<sub>2</sub> |
| Market value | MV<sub>0</sub> | MV<sub>1</sub> | MV<sub>2</sub> |

MV<sub>1</sub> = CF<sub>2</sub> / ( 1 + r )<sup>1</sup>
MV<sub>0</sub> = CF<sub>1</sub> / ( 1 + r )<sup>1</sup> +  CF<sub>2</sub> / ( 1 + r )<sup>2</sup> = ( MV<sub>1</sub> + CF<sub>1</sub>) / ( 1 + r )<sup>1</sup>
EI<sub>1</sub> = CF<sub>1</sub>) - ( MV<sub>0</sub> - MV<sub>1</sub>)

### 小结：经济收入vs会计收入

| - | 经济收入 | 会计收入 |
|----------|-----------------|--------------------------|
| 计算 | 现金 - 经济折旧 | 收入 - 支出 |
| 折旧 | 市值的降低 | 账面价值减少 |
| 融资成本 | 包含在折现率中 | 减去融资成本后得到净收入 |
