---
layout: post
title: CFA Level 2 经济 Part 2
categories: CFA 
---

## 目录
1. 利差交易（carry trade）
1. 汇率决定模型（exchange rate determination models）
1. 泰勒法则（Taylor rule）
2. 经济增长（economic growth）
3. 经济增长的决定因数（determinants for economic grwoth）


<br><br>

## 1. 利差交易（carry trade）
> 回顾无抛补利率平价（uncovered interest rate parity），利差交易只有在无抛补利率平价不成立的时候才能进行

- 当%△E(S) ≈ R<sub>A</sub> - R<sub>B</sub> 不成立时候，用利率低的货币作为借贷用货币（funding currency），兑换成去利率高利率低的货币投资
- 收益 = S/S' × ( 1 + R<sub>A</sub> ) - ( 1 + R<sub>B</sub> ) ≈ R<sub>A</sub> - R<sub>B</sub> - %△S
  - S/S' = 1 + %△S
  - 这个公式是用B货币借钱然后用A货币投资的情况
- 利差交易存在两个风险
  - 价格风险：投资金融资产时金融资产的市场价格与预期不一致的风险
  - 利率风险：两个货币之间的汇率变化与预期不一致的风险
- 利差交易适应在在市场波动小（market volatility）的情况使用

利差交易的风险：

- 汇率风险（currency risk）：借贷用货币（funding currency）可能会大幅升值，使得利差交易不再有利润
- 崩盘风险（crash risk）：回报的概率分布曲线（return distribution）的偏度是负数（negative skewness），峰度大于0（excess kurtosis）——意味着产生较大损失的概率较大（high probability of large loss）

利差交易的风险管理（risk management）：

- 市场波动过滤（volatility filter）：当市场市场波动屡到达某一个阈值（threshold），则取消（逆转）利差交易
- 定价过滤（valuation filter）：设定一个定价区间（valuation band），当其中一个货币贬值或升值过度，则加仓（overweight）或减仓（underweight）

<br><br>

## 2. 汇率决定模型（exchange rate determination models）
- 蒙代尔-弗莱明模型（Mundell - Fleming model）
  - 只考虑短期的影响
  - 考虑货币政策和财政政策的影响
- 货币论（Monetary approach）
  - 考虑短期和长期的影响
  - 只考虑货币政策的影响
- 资产市场说（Asset market (portfolio balance model)）
  - 只考虑长期的影响
  - 只考虑财政政策的影响

> 考试主要考蒙代尔-弗莱明模型本身，关于货币论和资产市场说只考他们和蒙代尔-弗莱明模型的区别

<br><br>

### a）蒙代尔-弗莱明模型（Mundell - Fleming model）
- 蒙代尔-弗莱明模型（Mundell - Fleming model）分析货币政策（monetary policy）和财政政策（fiscal policy）对于利率的影响，进而影响汇率
- 体现了三元悖论（the impossible trinity）的现象
- 不考虑通货膨胀的影响，只关注短期

**三元悖论（the impossible trinity）**

- 固定汇率（fixed exchange rate）
- 高资本流动性（high capital mobility）
- 独立的货币政策（independent monetary policy）

不能同时获得

**蒙代尔-弗莱明模型一共考虑了四种情况：**

|           -            | Flexible exchange rate | Fixed exchange rate |
|:---------------------:|:----------------------:|:-------------------:|
| High capital mobility |           (1)          |         (3)         |
|  Low capital mobility |           (2)          |         (4)         |

#### （1）浮动汇率制 + 资本自由流动

**货币政策（影响资本账户）：**

- 扩张的货币政策（expansionary monetary policy）- 本币贬值：
导致利率下降，投资者投资海外市场，资本的流出，本币需求降低，本币贬值
- 紧缩的货币政策（contractionary monetary policy）- 本币升值：
相反

**财政政策（影响资本账户和经常账户，但是资本账户影响大于经常账户的影响）：**

- 扩张的财政政策（expansionary fiscal policy）- 本币升值：
  - 资本账户的影响 > 经常账户的影响
  - 资本账户：
 降低税收，扩大政府支出，产生挤出效应（crowding out effect），利率上升，资本流入，本币本币需求增加，本币升值
  - 经常账户
 政府购买力增加，本国物价上涨，刺激进口消费，贸易逆差，然后本币贬值
- 紧缩的财政政策（contractionary fiscal policy）- 本币贬值：
相反

#### （2）浮动汇率制 + 资本不能自由流动

**货币政策（无影响）：**

- 扩张的货币政策 - 无变化：
导致利率下降，但是资本不能流出，所以对于本币需求不影响，本币价值不变
- 紧缩的货币政策（contractionary monetary policy）：
相反

**财政政策（资本账户无影响，影响经常账户）：**

- 扩张的财政政策 - 本币贬值：
  - 资本账户：
  降低税收，扩大政府支出，产生挤出效应（crowding out effect），利率上升，但是因为资本无法流入，本币需求不影响，本币价值不变
  - 经常账户：
  政府购买力增加，本国物价上涨，刺激进口消费，贸易逆差，然后本币贬值
- 紧缩的财政政策 - 本币升值：
相反

#### （3）固定汇率制 + 资本自由流动

**货币政策（实际上无法实施）：**

- 三元悖论
- 扩张的货币政策- 无效：
扩张的货币政策导致利率下降，投资者投资海外市场，资本的流出，本币需求降低，本币贬值，政府为了维持汇率，开始买入货币，所以等于是实施紧缩的货币政策，抵消了原本的扩张的货币政策的效果
- 紧缩的货币政策- 无效：
相反

**财政政策（影响资本账户）：**

- 扩张的财政政策 - 被动的实施扩张的货币政策
  - 只考虑资本账户，因为资本账户的影响处于主导地位：
 降低税收，扩大政府支出，产生挤出效应（crowding out effect），利率上升，资本流入，政府介入降低汇率，大量买入外币，被动的实施了扩张的货币政策
- 紧缩的财政政策 - 被动的实施紧缩的货币政策
相反

#### （4）固定汇率制 + 资本不能自由流动

**货币政策（无影响）：**

- 三元悖论
- 扩张的货币政策 - 被动的实施紧缩的货币政策：
导致利率下降，但是资本不能流出，所以对于本币需求不影响，本币价值不变
- 紧缩的货币政策：
相反

**财政政策（资本账户无影响，影响经常账户）：**

- 扩张的财政政策 - 被动的实施紧缩的货币政策
  - 因为资本不能只有流动，所以不会影响资本账户，只考虑经常账户
 政府购买力增加，本国物价上涨，刺激进口消费，贸易逆差，然后本币贬值，政府介入，大量买入本币，被动的实施紧缩的货币政策
- 紧缩的财政政策 - 被动的实施紧缩的货币政策
相反

#### 小结

| Float/Fix | Monet | Fiscal |  H Cap Mo  |  L Cap Mo  |
|:---------:|:-----:|:------:|:----------:|:----------:|
|   Float   | Expan |  Expan |  Uncertain | Depreciate |
|   Float   | Expan |  Contr | Depreciate |  Uncertain |
|   Float   | Contr |  Expan | Appreciate |  Uncertain |
|   Float   | Contr |  Contr |  Uncertain | Appreciate |
|    Fix    |  N/A  |  Expan |  Exp Mone  |  Con Mone  |
|    Fix    |  N/A  |  Contr |  Con Mone  |  Exp Mone  |

<br><br>

### b）货币论（Monetary approach）
- 蒙代尔-弗莱明模型不考虑通货膨胀的影响，仅仅是短期影响
- 货币论考虑短期和长期的变化，但是只考虑货币政策的影响
- 货币论（Monetary approach），假设经济输出恒定（output is fixed），所以货币政策主要影响通胀率，进而影响汇率
- 货币涉及到两个模型：
 - 纯货币模型（pure monetary model）
 - 多恩布什汇率超调模型（Dornbusch overshooting model）

#### （1）纯货币模型（pure monetary model）

- 假设：经济输出恒定（output is fixed）
- 假设：相对购买力平价（relative purchasing power parity）在任何时候成立
- 所以如果某一个国家的通货膨胀，其货币贬值（名义汇率的贬值）
- 因为假设相对购买力平价成立，实际汇率水平不变
- 通货膨胀的效果需要长期才能见效，所以纯货币模型分析的长期的状态

> 相对购买力平价（purchasing power parity）：part 1 中提及，汇率变化等于通胀率之差

#### （2）多恩布什汇率超调模型（Dornbusch overshooting model）

- 假设：经济输出恒定（output is fixed）
- 假设：短期物价水平存在粘性，变化需要时间，所以相对购买力平价（relative purchasing power parity）在短期不恒定

短期(in short term)：
扩张的货币政策，刺激经济降低利率，导致资本外流，进而贬值（通货膨胀尚未产生）

长期（in long term）：
扩张的货币政策，造成通货膨胀，进而贬值

为什么叫做超调模型？

- 在短期，货币的贬值幅度受到了双重影响，名义汇率和实际汇率都下降了（in the short term, the depreciation of currency is greater than the depreciation implied by PPP (i.e. overshoot the long-run)）
- 在长期，汇率最终将恢复到相对购买力平价的计算值的位置（均衡实质汇率（equilibrium real exchange rate）重新返回到历史水平）

<br><br>

#### c）资产市场说（Asset market (portfolio balance model)）
- 蒙代尔-弗莱明模型只考虑短期变化
- 资产市场说（Asset market (portfolio balance model)）只考虑长期

**资产市场说（Asset market (portfolio balance model)）**

长期的扩张的财政政策，刺激国民消费趋向于进口，贸易逆差，贸易逆差需要资本账户盈余来抵消，政府购入国外债券，外债规模增加，投资者开始对国家的经济持续性怀疑，本币贬值

政府有两个选择：

- 进而使用紧缩的财政政策，此举可能会遏制经济增长，而且这个过程会导致本币贬值
- 印钞（monetize its debt），收取“通货膨胀税”来缓解外债压力，这个过程也会导致本币贬值
- 在蒙代尔-弗莱明模型，扩张的财政政策导致本币升值（假设资本自由流动）
- 蒙代尔-弗莱明在适用于短期，资产市场说适用于长期

<br><br>

## 3. 泰勒法则（Taylor rule）

> 在组合part 2 中涉及收益率曲线（yield curve）时简短的谈到过泰勒法则（Taylor rule）是如何影响短期收益率的

政府设定短期名义利率目标的**泰勒法则（Taylor rule）**：
policy rate = RR<sub>f</sub> + I + α (I - I\*) + β (y - y\*)

> RR<sub>f</sub> = 预测实际无违约无风险利率 = 央行的政策中性实际利率 R<sub>n</sub>
> I: 实际膨胀率（actual inflation rate）
> I\*：目标膨胀率（target inflation rate）
> Y：实际GDP增长率取对（logarithmic level of actual real GDP）
> Y\*: 实际潜在GDP增长率取对（logarithmic level of potential real GDP）
> I - I\*：膨胀率缺口（inflation gap）
> y - y\*：输出缺口（output gap）
> α，β，由央行决定的比重，一般都是等于0.5

央行利用泰勒法则（Taylor rule）来决定政策利率目标（短期名义利率）（setting policy interest rates）

- 维持物价稳定（maintain price stability (inflation target)）
- 达到可持续水平的就业率的最大值（achieve the maximum sustainable level of employment）
- 美国的政策利率目标是通过改变federal fund rate，中国是通过影响信贷总量

美国政府估算RR<sub>f</sub>的方式，RR<sub>f</sub> = 政策中性实际利率 R<sub>n</sub> = 目标GPD增长率 + 目标通胀率

**代入（除去通货膨胀的）泰勒法则的实际汇率模型（real exchange rate model）**

real exchange rate <sub>(A/B)</sub> =
equilibrium real exchange rate
\+ ( r<sub>n,B</sub> - r<sub>n,A</sub> ) + α × [ ( I<sub>B</sub> - I\*<sub>B</sub> ) - (I<sub>A</sub> - I\*<sub>A</sub>) ]
\+ β × [ ( y<sub>B</sub> - y\*<sub>B</sub> ) - ( y<sub>A</sub> - y\*<sub>A</sub> ) ]
\- ( risk premium<sub>B</sub> - risk premium<sub>A</sub> )

> part 1 提到过实际汇率是如何计算而得的
>
> **国家如何通过影响外汇市场影响资本流动**

> 短期来看，实质汇率在长期均值回归平衡水平上下波动（fluctuate around）
> > 前面均衡实质汇率（equilibrium real exchange rate）提到，因为短期内常常不成立，所以实质汇率在这个均值回归平衡水平上下波动

> real exchange rate <sub>(A/B)</sub> = equilibrium real exchange rate + ( real interest rate<sub>B</sub> - real interest rate<sub>A</sub> ) - ( risk premium<sub>B</sub> - risk premium<sub>A</sub> )

> 货币的实际价值和实际汇率之差呈现正相关，风险溢价之差呈现负相关

**所以实际汇率的增加可以由以下原因导致：**

- 均衡实质汇率改变（equilibrium real exchange rate increase）
- B货币相对于A货币的政策中性实际利率增加（policy-neutral real interest rate in B relative to the A increases）
- B国和A国之间的膨胀率缺口变宽（inflation gap in B relative to the inflation gap in A increase）
- B国和A国之间的输出缺口变宽（output gap in B relative to the output gap in A increase）
- B货币的资产的风险溢价相对A的降低（risk premium of B-denominated assets relative to A-denominated assets decreases）

**中央银行的干预（central bank intervention）**

- 确保本币不会过度升值（appreciate excessively）
- 在不影响货币价值的（without being hindered by their impact on currency values）前提下确保独立的的货币政策（independent monetary policies）
- 防止吸引过量（excessive inflow）的海外资本

**中央银行的干预有效性（effectiveness）**

- 发达国家，中央银行的干预能力相对弱
- 新兴市场国家（emerging market countries），中央银行的干预能力相对强
  - 因为他们拥有着足够的外汇储备（相对于该币的交易量而言）来影响本币的供需关系
  - 美国虽然外汇储备的绝对值大，但是相对于它的交易量来说还是不够的
 - 资本流动控制是否能成功取决于流动的规模和可持续性（size of capital flows and persistence）
 
 > 回顾前面提到的三元悖论（the impossible trinity），因为新兴市场国家央行想要确保汇率稳定来保证出口贸易，确保独立的货币政策能控制国家经济，只能牺牲资本流动性

**货币危机的预警信号（signs of currency crisis）**
> 非重点

- 巨额贸易逆差（terms of trade deteriorate）
- 官方储备的急剧下降（official foreign exchange reserves dramatically decline）
- 实际汇率远高于均衡实质汇率水平（real exchange rate is substantially higher than the mean-reverting level）
- 通货膨胀（inflation increases）
- 资本市场泡沫（equity markets experiecne a boom-bust cycle）
- 货币供给过量（money supply relative to bank reserves increases）
  - 中国房地产的高价
- 名义私人信贷上升（nominal private credit grows）

**外汇的技术分析（technical analysis）**
> 没考过

- 趋势分析的规则（trend-following trading rules）
- 分析做市商报价（FX dealer order books）
- 外汇市场衍生品（currency options market）
  - 如果看涨期权（call option）的价格看跌期权（put option）的价格高，市场的预期是货币的升值机会比贬值机会大

<br><br>

## 4. 经济增长（economic growth）

**经济增长的前提条件（preconditions for grwoth）**

- 储蓄和投资（savings and investment）
  - 中国目前有非常充足的储蓄率
- 金融市场和金融机构（financial markets and intermediaries）
- 政策稳定，法律健全（political stability, rule of law, and property rights）
- 人力资本（investment in human capital）
- 税收和管制（tax and regulatory systems）
- 自由贸易和无限制的资本流动（free trade and unrestricted captial flows）

**潜在GDP（potential GDP）**
在不进一步产生通货膨胀的基础上，能到达的最大的经济输出（maximum amount of output an economy can sustainably produce without indcuing an increase in the inflation rate）

**潜在GDP和股市的关系**

- %△P = %△( P / E ) + %△( E / GDP ) + %△GDP
- 长期来看%△( P / E ) ≈ 0，%△( E / GDP ) ≈ 0 → %△P = %△GDP

**潜在GDP和固定收益市场的关系**

- 如果实际GDP > 潜在GDP → 通货膨胀，债券价格下跌
- 潜在GDP增长的越快，信用风险越低（经济良好，偿还债务的能力强）

**潜在GDP和金融市场的关系**
更高的潜在GDP增长 → 即期消费增加 → 政府鼓励储蓄 → 真实利率增加 → 资产证实收益率增加

<br><br>

## 5. 经济增长的决定因数（determinants for economic grwoth）

<br><br>

### a）【原始公式】柯布-道格拉斯生产函数（Cobb-Douglas production function）
Y = T × K<sup>α</sup> × L<sup>1-α</sup>

>T：全要素生产力（total factor productivity），反映了国家的技术水平（technological progress）
α：资本对于产出的贡献度
规模报酬不变（constant returns to scale）：资本对于产出的贡献度 + 人力资本对于产出的贡献度 = 1

> - 如果将所有的要素都提高一个固定的百分比，产出也提升一个相同的百分比

<br><br>

### b）【变体】劳动生产率（output per worker, labor productivity, GDP per capita）
> 将柯布-道格拉斯生产函数（全要素生产力函数）左右两边同时除以人力资本L，即得到了单位工人的输出

Y/L = T × ( K / L )<sup>α</sup> → y = T × k<sup>α</sup>

- 假设L和α保持不变，输出的增加可以由资本深化（capital deepening）或者科技进步（improving technology）
- 由于α < 1, 额外的资本投入产生的产出是递减的（diminishing effect）
- 发达国家的一般有较高的 K / L和较低的 α，所以资本深化的收益较低，需要依赖科技进步
- 发展中国家可以依赖资本深化获得短期的生产力提高

在稳定状态下（平衡状态下），资本输入带来的边际产出（marginal product of capital）等于资本边际成本（marginal cost of capital，用r表示，其实就是资本的必要收益率 required return）：

marginal product of capital = r → α = r × K / Y

> 使用原始的柯布-道格拉斯生产函数，
> Y = T × K<sup>α</sup> × L<sup>1 - α</sup>
> 对K进行求导，
> △Y / △K = T × L<sup>1 - α</sup> × α × K<sup>α - 1</sup>
> 变形，
> △Y / △K = α / K × ( T × K<sup>α</sup> × L<sup>1 - α</sup>)
> 因为Y = T × K<sup>α</sup> × L<sup>1 - α</sup>
> △Y / △K = α / K × Y
> 当△Y / △K = r 时达到稳定状态，故得到公式
> α = r × K / Y

- 当MPK > r，经济发展会因为资本深化而受益
- 当MPK = r，资本深化不再有效，生产力的提高只能依赖科技进步

<br><br>

### c）【变体】增长会计法（growth accounting equation）
Y = T × K<sup>α</sup> × L<sup>1-α</sup> →
△Y / Y = △T / T + α × △K / K + ( 1 - α ) × △L / L
> 将柯布-道格拉斯生产函数（全要素生产力函数）对Y进行求导

>△Y / Y: 潜在GDP的增长率
△T / T：科技的长期增长率
△K / K：资本的长期增长率
△L / L：人力资本的长期增长率

由于生产要素的变化缓慢，所以将来的期望增长率可以用过去的过去的增长率带入

<br><br>

### d）【变体】劳动生产率增长会计法（labor productivity growth accounting equation）
> 将劳动生产率对y进行求导

Y = yL → △Y / Y = △y / y + △L / L
> △y / y：劳动生产率的长期增长率
> △y / y体现了资本深化和科技进步影响

y =TK<sup>α</sup> → △y / y = △T / T + α × △k / k

**自然资源（natural resource）**
自然资源多寡对于经济的影响是复杂的

- 有些自然资源丰富的国家经济发展迅速，比如澳大利亚
- 有些自然资源丰富的国家经济发展缓慢，比如沙特阿拉伯，委瑞内拉
  - 没有合理发展别的必要产业
  - 荷兰病（Dutch disease）：来自全球对于自然资源的需求，导致货币升值，使得别的行业，尤其是生产业，没有竞争力

**劳动力（labor supply）**
影响劳动力供给的因素：

- 人口增长（population growth）：
年轻人口越多，潜在经济增长力更高
- 劳动参与（labor force participation）：
更多的女人进行工作可以提高劳动参与
- 外来移民（immigration）
衰减的劳动力问题的潜在解决方案
- 平均工作时长（average hours worked）
目前的趋势是降低工作时间

**人力资本（human capital）** - 劳动力的质量

- 教育（education）和在职培训（increase work experience）
- 受教育的工人进行创新（innovate），产生溢出效应（spillover effect）

**实体资本（physical capital）**

- 信息，计算机，通讯资本（information, computers, and telecommunications capital (ICT)）
- 非信息，计算机，通讯资本（non-ITC）

为什么资本投入依然可能促进经济增长？

- 发展中的经济（developing economies）有相对较低的人均资本水平（relatively low capital to labor ratio）
- 一些资本投资可以促进科技进步（influence technological progress），因此增加了全要素生产力，促进经济发展

技术水平的发展（technological development）

- 发达国家大部分的花费用在R&D上，因为资本的充足和缓慢人口增长
- 未完全发达国家常常复制发达国家的科技创新，能够用相对于GDP来说更少的R&D花费