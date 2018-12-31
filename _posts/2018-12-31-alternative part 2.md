---
layout: post
title: CFA Level 2 另类投资 Part 2
categories: CFA 
---

## 目录
1. 公开交易的房地产证券（publicly traded real estate securities）
2. REIT和REOC的估值方法（evaluation）
3. 私募股权基金（private equity）
4. 私募股权基金（private equity）与投资组合成员公司（portfolio companies）

<br><br>

## 1. 公开交易的房地产证券（publicly traded real estate securities）

<br><br>

CFA主要研究两种公开交易的房地产证券（publicly traded real estate securities）

1. 房地产经营公司（real estate operating company）
2. 房地产投资信托（real estate investment trust (REITs)）

**房地产经营公司（real estate operating company）**

- 不存在免税
- 不出租房产，只是出售房产

**房地产投资信托（real estate investment trust (REITs)）**

- 免除企业收入税（corporate income tax）
- 75%的收入来自于房地产，并且需要将几乎全部的收入发放给股东
- REITs的股利收益率（dividend yield）一般比别的资产要高
- 收入波动性低（low income volatility）
- 再融资频繁（frequent secondary equity offering），因为绝大部分利得都被派发出去了

相对于私有的房产投资，购买房地产的优点

- 流动性高
- 较低的最低投资要求
- 有限责任
- 投资的范围更大，更有可能投资优秀的资产
- 自带房产管理
- 分散化投资

REOC的优势

- 投资的灵活性，REIT限于租金收入
- 可以保留收入
- 可以使用杠杆

GDP对于REIT的收入的影响最大。

<br><br>

## 2. REIT和REOC的估值方法（evaluation）

<br><br>

**估值的三种方法：**

- 每股净资产值（net asset value per share (NAVPS)）
- 相对值（relative value(RV)）
- 现金流折现（discounted cash flow(DCF)）

<br><br>

### a）每股净资产值（net asset value per share (NAVPS)）：

- 计算资产和负债之间的差值，使用当时的市场价值而不是会计账面价值
- 净运营收入（NOI）是未来一年的预测

计算方法：

（今年预计的NOI（NOI<sub>this year</sub> ） × 增长率（ 1 + g ）/ 假设的资本率（assumed cap rate） + 现金和应收账款（cash and accounts receivable） - 债务和其他负债（debt and other liabilities））/ 流通股份（shares outstanding） = 每股净资产（NAV per share）




### b）相对值（relative value(RV)）
相对值（relative value(RV)）有两种方法：

- 价格营运现金流量比（price to funds from operations (P/FFO)）
- 价格调整后营运现金流量比（price to adjusted funds from operations (P/AFFO)）

**营运现金流量（funds from operations）的计算（和现金流量表的计算类似）**

会计净收入（accounting net earnings）
+ 折旧成本（depreciation expense）
+ 递延税项（deferred tax expenses / liabilities）
- 来自资产出售和债务重组的收入/支出(gains / losses from sales of property and debt restructuring)
= 营运现金流量（funds from operations）

**调整后营运现金流量（adjusted funds from operations）的计算（和公司自由现金流的计算类似）**

营运现金流量（funds from operations）
- 非现金租金直线摊销（non-cash straight-line adjustment）
- 经常性维护性资本支出和租赁成本（recurring maintenance-type capital expenditures and leasing cost）
= 调整后营运现金流量（adjusted funds from operations）

**非现金租金直线摊销（non-cash straight-line adjustment）：**
租金的实际接收日期和会计结算日不一定一致，所以需要做一定的调整

**经常性维护性资本支出和租赁成本（recurring maintenance-type capital expenditures and leasing cost）：**
用于维持房产价值的支出

> 公司自由现金流（cash flow to the firm）
> 净收入（net income） + 非现金支出（non cash charge） + 利息支出（interest  ( 1 - tax rate )）- 固定资本投资（fixed capital investment） - 运营资金（working capital investment）

小结：

1. 相对P/FFO，P/AFFO对于收入的测量更准确，因为它考虑到维持房产正常收入的必要支出，但是P/AFFO的波动更大
2. P/AFFO和P/FFO一般是使用的当前股价和未来一年的AFFO和FFO的比值
3. P/FFO类似于REIT投资界的P/E，AFFO可以当做是现金流的粗略估计

P/AFFO和P/FFO的优点：

1. 全球广泛使用
2. 便于和其他投资资产的比较
3. 数据容易获取，通过Bloomberg或者Thomson Reuters

P/AFFO和P/FFO的缺点：

1. 并不能有效的计算所有类型的房产类型，比如还没有投入使用的空地（没有收入，所以没有现金流量）
2. P/FFO没有考虑房产的支出，所以不同房产的可比性不强，P/AFFO的波动性更大，可比性也不高。
3. 会计的数据可能会被人为操纵过

<br><br>

### c）现金流折现（discounted cash flow(DCF)）

现金流折现（discounted cash flow(DCF)）的方法的名称叫做股息现金流模型（dividend cash flow model）

**股息现金流模型（dividend cash flow model）**

- 将股息现金流进行折现
- 对数据的敏感度高（可能会偏离现实）

<br><br>

> ### 例题：
Calculate the value of of a REIT share
Lucinda Crabtree, CFA, is an asset manager that is interested in diversifying the portfolio she manages through an investment in an office building REIT. Crabtree wants to value the potential investment using for different approaches as of the end of 2013, as follows:

> - Approach 1: Net asset value
- Approach 2: Price-to-FFO
- Approach 3: Price-to-AFFO
- Approach 4: Discounted cash flow

> numbers in millions.
>
| 80    | Estimated 12 months cash NOI                     |
|-------|--------------------------------------------------|
| 70    | Funds from operations                            |
| 65    | Cash and equivalents                             |
| 35    | Account receivable                               |
| 400   | Debt and other liability                         |
| 5     | Non-cash rents                                   |
| 15    | Recurring maintenance-type capital expenditures  |
| 10 m  | shares outstanding                               |
| $5.00 | Expected annual dividend next years (2014)       |
| 2%    | Dividend growth rate in 2015 and 2016            |
| 1%    | Dividend growth rate (from 2017 into perpetuity) |
| 8%    | Assumed cap rate                                 |
| 10    | Office subsector average P/FFO multiple          |
| 14    | Office subsector average P/AFFO multiple         |
| 9%    | Crabtree's applicable cost of equity capital     |
| 2%    | Risk-free rate                                   |

> ### Answer:
>
> ### Approach 1: Value of a REIT share using net asset value approach

| 80     | Estimated cash NOI                                   |
|--------|------------------------------------------------------|
| 8%     | Assumed cap rate                                     |
| 1,000  | Estimated value of operating real estate (80 / 0.08) |
| 100    | Plus cash + accounts receivable (65 + 35)            |
| 400    | Less debt and other liabilities                      |
| 700    | Net asset value                                      |
| 10     | Shares outstanding                                   |
| $70.00 | NAV / share                                          |

> The REIT share value using the net asset value approach is thus $70.
>
> - Note that no adjustment for non-cash rents was required in this case because we began with an estimate of cash NOI
>
> ### Approach 2: Value of a REIT share using price-to-FFO approach
> The value per share for this REIT using price-to-FFO valuation is computed as follows:
>
| $70   | Funds from operations (FFO)   |
|-------|-------------------------------|
| 10    | Shares outstanding (millions) |
| $7.00 | FFO / share = $70 m / 10 m    |

> Applying the office subsector average P/FFO multiple of 10× yield a value per share of:
> $7.00 × 10 = $70.00
> The REIT share value using the price-to-FFO approach is thus $70
>
> ### Approach 3: Value of REIT share using price to AFFO approach
>
| $70 | Funds from operations (FFO)                          |
|-----|------------------------------------------------------|
| $5  | Less non-cash rents                                  |
| $15 | Less recurring maintenance-type capital expenditures |
| $50 | AFFO                                                 |
| 10  | Shares outstanding (million)                         |
| $5  | AFFO / share                                         |
| 14× | Property subsector average P/AFFO multiple           |

> Applying the office subsector average P/AFFP multiple of 14× yield a value per share of $55 × 14 = $70
> The REIT share value using the price-to-AFFO approach is thus $70
>
> ### Approach 4: Value of REIT share using discounted cash flow approach
>
|          | 2014  | 2015  | 2016  |
|----------|-------|-------|-------|
| Dividend | $5.00 | $5.10 | $5.20 |
> Present value in 2016 of dividends stream beginning in 2017 = 5.20 ( 1 + 1% ) / ( 0.09 - 0.01 ) = 65.65
> These dividends are discounted at rate of 9%.
> Value of a REIT share = PV (dividends for years 1 through n) + PV (terminal value at the end of year n)
> = PV<sub> 2014 dividend</sub> + PV<sub> 2015 dividend</sub> + PV<sub> 2016 dividend</sub> + PV<sub> 2017 and later dividends (terminal value)</sub>
> = $5.00/1.09 + $5.10/1.09<sup>2</sup> + $5.20/1.09<sup>3</sup> + $65.65/1.09<sup>3</sup> =$63.59
> The REIT share value using the discounted cash flow approach is thus $63.59

<br><br>

## 3\. 私募股权基金（private equity）

<br><br>

**相关概念：**

- 私募股权投资者（private equity investor）：向私募股权基金提供资金的外界投资者
- 私募股权基金（private equity fund）：进行私募股权投资的相关交易的载体
- 投资组合成员公司（portfolio companies）：私募股权投资的公司

**私募股权的分类（classification of private equity）**

- 风险投资 （venture capital (VC)）
投资处于早期阶段的公司，目前收入极地但是存在良好发展前景
- 并购投资（buyout）
买入整个公司
- 特殊情况（special situation）
问题证券（distress securities）投资，一次性机遇（one-time opportunities）投资，等等

**风险投资 （venture capital (VC)）vs 并购投资（buyout）**

- VC投资更多的是处于早期阶段的公司
- VC可能存在行业偏好（specialized industry focus），并购投资类PE一般选择有可预见的现金流模式（predictable cash flow pattern）的公司
- VC寻找的是收入的增长（revenue growth），并购投资类PE的寻找的是息税前利润和税息折旧及摊销前利润的增长（EBIT and EBITDA growth）

**私募股权投资产生价值的方式**

- 对公司进行整改（re-engineer），使其经营更加有效
- 获得有利协议（favorable term）的债券融资
  - PE公司可能有好的借贷渠道
- 使得投资组合成员公司的管理层和基金的利益趋于一致（align the interests）
  - 建立长期奖励方案（long-term incentive package）
  - 制定相应的合约条款（contractual clause）

<br><br>

## 4\. 私募股权基金（private equity）与投资组合成员公司（portfolio companies）

<br><br>

**私募股权投资基金和投资组合成员公司之间的合约条款（contractual clause）**

- 在管理结构（governance structure）方面
  - 公司董事会的席位（corporate board seat）：PE将参与公司董事会
  - 保留事项（reserved matters）：保留对重要变动的控制权和否决权（veto），例如商业计划（business plan），并购（acquisition），自愿剥离（divestiture）
- 在利润的分配（distribution）方面
- 在激励机制（incentive）和限制条件（constrain）方面
  - 酬薪（compensation）
  - 一系列的期权奖励（ratchet(option)）
  - 跟随权（tag-along）和强卖权（drag-along）：在第三方公司对投资组合成员公司进行购买时，PE有权选择按照相等条件卖出控制股份或者强制卖出控制股份
  - 盈利能力支付计划（earn-out）：PE公司会分阶段的注入资本，金额会根据业绩进行调整
  - 竞业限制条款（non-competing clause）：在一定时限内防止管理层参与竞争者的公司

**并购投资（buyout）有三种类型：**

- 管理层收购（management buyout (MBOs)）
- 杠杆收购（leveraged buyouts (LBOs)）
- 恶意收购（hostile takeovers）

**杠杆收购（leveraged buyouts (LBOs)）利用贷款融资进行收购，贷款的类型可以是：**

- 优先债（senior debt）
- 高收益债券/垃圾债券（high yield bond）
- 夹层融资（mezzanine finance）
  - 属于权益和债券投资的各类组合混合形式的泛称

**杠杆收购模型（LBO model）**

- 资金的来源：
  1. 目标公司的现金流预测（cash flow forecast of target company）
  2. 融资提供方的期待收益率（expected return from the providers of financing）
  3. 可用的融资资金量（amount of available financing）
- 资金的去处：
  1. 权益内部收益率的变化敏感度的预计（expected IRR sensitivity of equity）
  2. 满足目标收益率的最大可支付价格（maximum payable price satisfying target return）

退出（exit）的日期是计算PE收益率一个重要因素

**风投的投资估值**

- 交易前估值（pre-money valuation (PRE): 投资（financing or investment (INV)）前公司的价值
- 交易后估值（post-money valuation (POST)）：投资（financing or investment (INV)）后公司的价值
- POST = PRE + INV
- 控股比例可以由INV / POST算出

**风投的投资估值问题（issues in VC transactions）**

- 交易前估值会受到协商（negotiation）的影响，未来的融资会稀释（dilute）控股比例
- 因为被投资公司的现金流存在高度不确定性，所以现金流折现（discounted cash flow）并不可靠
- 因为被投资公司可能非常独特，所以同行对比（comparable quoted companies）并不可靠

**并购投资的投资估值问题（issues in buyout transaction）**

- 因为现金流更容易预测，所以收入型的估值方式（income-based approach）使用的更多
- 投资初始的高杠杆率和往后逐步下降的刚刚率是估值时需要考虑的因素
- 估值时通常使用同类型上市公司进行比较

**小结**

| 问题     | 杠杆并购                             |   风险投资                             |
|----------|--------------------------------------|--------------------------------------|
| DCF      | 经常使用                             | 较少使用                             |
| 同业对比 | 和DCF一并用                          | 难以应用                             |
| 债券杠杆 | 高                                   | 低                                   |
| 收益主因 | 收入增长，公司价值增加，债务负担程度 | 交易前估值，投资金额，股份的稀释程度 |

**退出（exit）**

- 大部分PE在投资前已经决定了退出方案，并且将退出的结果作为分析投资收益的重要因素
- 退出价值（exit value）
  - 即将退出，使用近期的收益倍数（multiple）
  - 退出还需要一段时间，使用预测的收益倍数（multiple）
- 情景分析（scenario analysis）

**四种退出方式（four exit routes）**

- 首次公开募股（initial public offering）
  - 优点：估值高，资本量大，有可能能吸引更好的管理者
  - 缺地：程序复杂，花费高
  - 首次公开募股的时机是重要的考虑因素
- 二级市场（secondary market）
  - 在二级市场交易，收益仅次于首次公开募股，但花费也次之
- 管理层购回（management buyout）
  - 公司原有管理层购回公司的所有权
- 清算（liquidation）
  - 可能会对PE公司的公众形象造成负面的影响
  - 收益最低，费用最低
