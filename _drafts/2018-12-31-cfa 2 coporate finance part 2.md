---
layout: post
title: CFA Level 2 公司金融 Part 2
categories: CFA2级笔记
---

## 目录
1. 估值方法 2：经济收益（economic profit）
2. 估值方法 3：剩余收益（residual income）
3. 估值方法 4：索取权价值（claims valuation）
4. 资本结构（capital structure）
4. 资本结构理论（capital structure theory）
5. 资本结构的成本（cost）
6. 静态权衡理论（static trade-off theory）
7. 债券评级（debt ratings）
8. 评估资本结构（evaluating capital structure）
1. 股利政策理论（theories of dividend policy）
2. 影响股利政策的因素（factors affecting dividend policy）
3. 股利政策（payout policies）的类型
4. 股利政策：股票回购vs现金股利
5. 股利的安全性/持续性（dividend safety）

<br><br>

## 1\. 估值方法 2：经济收益（economic profit）
> 这里的收益是从公司的角度考虑，收益相等于是股东和债券人共同的收益

**经济增加值 / 经济收益（economic value added / economic profit）**

- = 税后营业收益（net operating profit after tax (NOPAT)）-  加权平均资本成本额（dollar WACC）
- = 息税前利润（EBIT） × （ 1 - 税率） - 加权平均资本成本（WACC） × 资本额（capital）
- 资本额 = 权益投资 + 债务投资

> 利润 - 融资成本（机会成本）

**市场增加值（market value added）：**

- 将每一期的经济增加值 / 经济收益折现并进行加总，相当于计算净现值（NPV），折现率为WACC
- 市场增加值（market value added）= 净现值（NPV）= Σ economic profit<sub>t</sub> / (1 + WACC)<sup>t</sup>
- 公司价值（V<sub>firm</sub>） = 市场增加值（market value added） + 投资额（investment）


## 2\. 估值方法 3：剩余收益（residual income）
> 这里的收益是从股东的角度考虑

剩余收益（residual income） = 股东净收益（net income<sub>t</sub>） - 股东要求权益收益率（r<sub>e</sub>）× 股东投入初始金额（B<sub>t-1</sub>）

> 股东所得利润 - 股东机会成本

- 净现值（NPV） = Σ residual income<sub>t</sub> / ( 1 + r<sub>e</sub> )<sup>t</sup>
- 权益价值（V<sub>E</sub>） = NPV + BV<sub>E</sub>


## 3\. 估值方法 4：索取权价值（claims valuation）

索取权价值法（claims valuation approach）基于 股权人和债权人的的索取权的价值之和等于公司价值 这一事实计算公司价值

- 债权人（debt holder）的现金流：
	- 债券融资成本（cost of debt）的折现
- 股权人（equity holder）现金流：
	- 权益融资成本（cost of equity）的折现
- 公司价值：
	- 债券现金流的现值 + 权益现金流的现值

索取权价值计算的是公司的价值，而不计算NPV

<br><br>

## 4\. 资本结构（capital structure）

公司的资本结构目标（objective），一般来说是指债务股本比（debt to equity ratio），是达到一个合理水平

- 达到最大化公司价值（firm value），最小化融资成本，即WACC
- 公司价值最大化，也就会达到股东价值的最大化，最终最大化股价
- 并不代表最大化EPS或者ROE
	- 因为公司价值还包含了未来产生回报的能力，EPS和ROE注重的是当前的情况

<br><br>

## 5\. 资本结构理论（capital structure theory）

1. 米勒 一 莫迪利安尼理论 1（无税）（Modigliani-Miller proposition I (no taxes)
2. 米勒 一 莫迪利安尼理论 2（无税）（Modigliani-Miller proposition II (no taxes)）
3. 米勒 一 莫迪利安尼理论 1（有税）（Modigliani-Miller proposition I (with taxes)）
4. 米勒 一 莫迪利安尼理论 2（有税）（Modigliani-Miller proposition II (with taxes)）

<br><br>

#### a）米勒 一 莫迪利安尼理论 1（无税）（Modigliani-Miller proposition I (no taxes)）：资本结构无关论（capital structure irrelevance proposition）

- **公司的价值不会受公司的资本结构的影响**
- 前提假设：
	- 投资有相同的现金流回报预期（agree on the expected cash flow）
	- 完美资本市场（perfect capital market），信息完全公开，交易无成本
	- 所有投资者可以以无风险利率借贷（borrow/lend at the risk-free rate）
	- 没有代理人成本（no agency costs），也就没有了代理人问题
	- 所有投资决策都是独立的（decisions are independent）

在米勒 一 莫迪利安尼理论I中

- 公司不会因为改变杠杆率（leverage）而产生价值
- 所以不存在最优资本结构
	- 存在杆杆的公司价值 = 不存在杠杆的公司价值

#### b）米勒 一 莫迪利安尼理论 2（无税）（Modigliani-Miller proposition II (no taxes)）：股东要求收益率和债务股本比存在线性关系（the cost of equity is a linear function of D/E）

- 从股权人的角度来看，公司的杠杆率越高，股东需要承担的风险越高
- 股东的要求收益率 r<sub>E</sub> = r<sub>0</sub> + ( r<sub>0</sub> - r<sub>D</sub> ) × ( D / E )
- 假设：
	- 完美市场（perfect market），债权人对于资产和收入的索取权（claim）比股权人优先级高

#### c）米勒 一 莫迪利安尼理论 1（有税）（Modigliani-Miller proposition I (with taxes)）：杠杆最大化的时候价值最大（value is maximized at 100% debt）

-	因为借贷会产生税盾（tax shield）给公司带来利益，所以最佳融资配置是100%借贷
-	V<sub>Leverage</sub> = V<sub>Unleverage</sub> + t × d

#### d）米勒 一 莫迪利安尼理论 2（有税）（Modigliani-Miller proposition II (with taxes)）：完全依赖借贷融资时WACC最小（WACC is minimized at 100% debt）

- r<sub>E</sub> = r<sub>0</sub> + ( r<sub>0</sub> - r<sub>D</sub> ) × ( D / E ) × ( 1 - t )

#### e）小结

| - | Without taxes | With taxes |
|---------------|------------------------------------------------------------------|-------------------------------------------------------------------------|
| r<sub>e</sub> | 变化快 | 变化慢 |
| 公司价值 | 不变 | 全债最优 |
| WACC | 不变 | 全债最优 |
| 理论 1 | V<sub>L</sub>=V<sub>U</sub> | V<sub>L</sub>=V<sub>U</sub>+t×D |
| 理论 2 | r<sub>e</sub>=r<sub>0</sub>+(r<sub>0</sub>-r<sub>D</sub> )×(D/E) | r<sub>E</sub> = r<sub>0</sub>+(r<sub>0</sub>-r<sub>D</sub>)×(D/E)×(1-t) |

\*米勒 一 莫迪利安尼理论不考虑财务困境成本和破产风险（financial distress/bankruptcy）

<br><br>

## 6\. 资本结构的成本（cost）

<br><br>

#### a）财务困境成本（financial distress cost）
在公司的利润降低时，将产生的金融负担

- 财务困境的期望成本（expected costs of financial distress）分为两个部分
	- 在真正遇到财务困境和破产时产生的花费（cost of financial distress and bankruptcy）
	- 遇到财务困境的概率（probability of financial distress）

在真正遇到财务困境和破产时产生的花费

- 直接花费（direct cost）
	- 与破产相关的现金花费
- 间接花费（indirect cost）
	- 损失的投资机遇（foregone investment opportunities），损失的顾客，债权人，供应商，已经员工的信心（losing trust of customers, creditors, suppliers, and employees）

遇到财务困境的概率（probability of financial distress）

- 该概率随杠杆的程度增加而增加（probability increases as the degree of leverage increase）
- 管理层和公司治理结构质量（quality of management and corporate governance structure）

#### b）代理人权益成本（agency cost of equity）
由于公司管理层（company's managers）和所有者（owners）之间的利益冲突（conflict of interest）产生的花费

- 管理者的股份（stake）越少，花费越高

**净代理人权益成本（net agency cost of equity）由以下三个方面决定：**

1. 监管成本（monitoring costs）
	- 为了监管（supervising）管理层的业绩表现带来的成本
2. 联结成本（bonding costs）
	- 为了激励管理层是在为股东利益而工作而带来的成本
3. 残余损失（residual losses）
	- 因为监管和联结机制（mechanism）并不完美导致的损失

代理人成本问题，带来的结论：

- 公司治理越优良，代理人成本越低
- 杠杆率越高，代理人成本越低

#### c）信息不对称成本（cost of asymmetic infomation）
由于公司管理者比投资者拥有更多的信息

- 因为信息的不对称，股权人和债券人要求的收益率会更高

例子：

- 潜在不良行为信号（negative signal）：股权融资
	- 管理层一般在股价高估的时候增发股票，在股价低估时倾向于不增发
- 潜在良好行为信号（positive signal）：债券融资
	- 管理层对于公司未来产生收入的能力有信心

**优先融资顺序理论（pecking order theory）**

管理层倾向于以最小化信息潜在信息披露（disclose less information）的方式融资

融资顺序：

1. 内部产生的权益（internally generated equity），例如：保留盈余（retained earnings）
2. 债券（debt）
3. 外部权益（external equity），例如：股票增发（newly issued shares）

由优先融资顺序理论，得出结论，资本结构是多个单次融资决策的副产品（capital structure is a by-product of the individual financing decisions）

<br><br>

## 7\. 静态权衡理论（static trade-off theory）

<br><br>

在债务融资带来的经济收益和可能的财务困境压力做权衡

V<sub>L</sub> = V<sub>U</sub> + (t × d) - PV (cost of financial distress)

静态权衡理论（static trade-off theory）的关键点（key points）：

- 税盾（tax shield）会给公司产生价值（add value）
- 财务困境成本（cost of financial distress）会使公司损失价值
- 当税盾产生的增值和财务困境成本导致的减值达到平衡时（balanced），公司达到最小化融资成本下的最大化价值（max value with lowest cost of capital）

**目标资本结构（target capital structure）**

- 长期来看，公司将使用的资本结构
- 公司管理管理者想要最大化公司价值
	- 目标资本结构（target capital structure） = 最优资本结构（optimal capital structure）
- 短期内，可能会在目标资本结构上下波动（fluctuate around the target），原因有两个：
	- 市场机遇（market opportunities）：管理层借用市场出现的偶然机遇，例如证券的定价错误，做出有利于公司的融资决策
	- 市场价值波动（market value fluctuation）：市场波动导致公司的股票价值和债券价值变化

<br><br>

## 8\. 债券评级（debt ratings）

公司管理层在进行借贷融资过程中需要考虑公司的债务评级问题

- 当杠杆率上升时（leverage rises），评级机构倾向于下调公司债券评级（rating），以反映公司上升的信用风险（higher credit risk）
- 更低的评级（rating）意味着更高的融资成本（cost of capital）

因为债券评级影响了融资成本，管理层常常将债券评级维持在特定的债务评级水平之上

<br><br>

## 9\. 评估资本结构（evaluating capital structure）

<br><br>

分析师在评估公司的资本结构（evaluating capital structure）需要考虑一下三点：

- 长期以来公司的资本结构变化（change）
- 具有类似经营风险的竞争者（competitors with similar business risk）的资本结构
- 公司特有的因素（company-specific factors）

**国际市场的公司的资本结构特点**

国际上杠杆率的不同（international differences in leverage）

- 总债务（total debt）：日本，意大利，法国的公司相比美国和英国有更高比例的总债务
- 债务期限（debt maturity）：北美的公司相比日本的公司债务的期限更长
- 新兴市场（emerging market）：相比处在新兴市场（emerging market）的公司，发达国家的公司的总债务比例更高，期限更长

**国际市场的资本结构差别的三个原因：**

1. 制度和法律因素（institutional and legal factors）
2. 金融市场和银行系统因素（financial market and banking system factors）
3. 宏观经济因素（macroeconomic factors）

1\. 制度和法律因素（institutional and legal factors）

- 法律系统有效性（strength of legal system）
	- 在法律系统较弱的国家里的公司，有着更高的代理人成本，因此有更高的杠杆率和更短的债券期限
- 信息不对称（information asymmetry）
	- 高度信息不对称导致管理层倾向于使用更多的借债
- 税收
	- 税盾鼓励借债
	- 股息税率低的时候，公司倾向于股权融资，因为投资者需要的收益率下降

2\. 金融市场和银行系统因素（financial market and banking system factors）

- 市场流动性（liquidity of capital markets）
  - 如果资本市场有更高的流动性（liquid）和更大规模（larger），在其中的公司的债务期限更长
- 银行系统的依赖（reliance on banking system）
  - 对银行系统的依赖更高国家，公司的平均杠杆水平越高
- 机构投资者的存在（presence of institutional investor）
  - 机构投资者可能有相对应的债券期限偏好（preferred maturity ranges）

3\. 宏观经济因素（macroeconomic factors）

- 通货膨胀
  - 高通胀率使得固定收益减值，所以公司更少地进行债券融资，而且债务期限更短
- GDP增长率
  - 高GDP增长率的国家，它的公司的债务期限更长

<br><br>

## 10\. 股利政策理论（theories of dividend policy）

<br><br>

**股利政策理论（theories of dividend policy）**

1. 股利无关理论（dividend is irrelevant to company value）
2. “在手之鸟”理论（bird in hand argument）
3. 税收厌恶（tax aversion）理论
4. 追随者效应（clientele effect）理论
5. 股利信号（signaling）理论
6. 代理人问题（agency issues）理论

<br><br>

#### 1\. 股利无关论（dividend is irrelevant to company value）

- 投资者可以自制股利（homemade dividend）
  - 通过抛售相应价值的股票获得现金

#### 2\. “在手之鸟”理论（bird in hand argument）

- 投资者偏好现金股利（cash dividend），因为存在确定性
- 发放股利的公司有更低的权益融资成本（lower cost of equity），因此公司价值更高

#### 3\. 税收厌恶（tax aversion）理论

- 投资者偏好税收低（incur lower tax）的方式
  - 如果股利的税率比资本利得（capital gain）的税率，投资者会偏好更低的股利支付率（dividend payout ratio）

#### 4\. 追随者效应（clientele effect）理论

不同的投资者有不同的股利政策偏好（desired dividend policy），因为：

- 所得税考虑（tax consideration）
  - 处于高税级（high tax bracket）的投资者倾向更低的股利
- 机构投资者（institutional investors）倾向
  - 一些机构投资者只会选择股利达到某个特定值的公司
- 个人投资者（individual investor）倾向
  - 一些个人投资者倾向于购买有股利的股票
- 追随者效应（clientele effect）理论和股利无关论（irrelevance）不矛盾
  - 改变股利政策只会改变客户类型

因为税收的存在，投资者会依照股利额进行相关的股票交易策略（tax effects the trading strategies in regard with dividend）

- **为保证对股东公平：**在股利派发前的抛售带来的收益（sell just before ex-dividend） = 在股利派发后的抛售带来的收益（sell just after ex-dividend）
  - （股利派发前）卖出价格 - 资本利得税 = （股利派发后）卖出价格 - 资本利得税 - 税后股利收入
  - P<sub>B</sub> - ( P<sub>B</sub> - P<sub>0</sub> ) × T<sub>CG</sub> = P<sub>A</sub> - ( P<sub>A</sub> - P<sub>0</sub> ) × T<sub>CG</sub> + D × ( 1 - T<sub>D</sub> )
- **股利派发前后产生的资本利得的税后收益 = 税后股利**：股利派发前后价差 = 税后股利收入 / （1 - 税率）
  - △P = P<sub>B</sub> - P<sub>A</sub> = D  × ( 1 - T<sub>D</sub> ) / ( 1 - T<sub>CG</sub> )
  - **变体：**△P × ( 1 - T<sub>CG</sub> ) = D × ( 1 - T<sub>D</sub> )
- **结论：** 如果
  - 资本利得税 = 股利税，股价下降幅度 = 股利
  - 资本利得税 < 股利税，股价下降幅度 < 股利
  - 资本利得税 > 股利税，股价下降幅度 > 股利

#### 5\. 股利信号（signaling）理论

第一次派发股利（a dividend initiation）

- 积极信号（positive signal）：公司对于发展前景表示乐观，对于未来收益预期乐观
- 负面信号（negative signal）：公司没有找到新的投资机会

超出预期的股利变动（unexpected dividend changes）

- （积极信号）超预期的增加（unexpected increase）：公司未来发展前景良好
- （负面信号）超预期的减少或者取消（unexpected increase or omission）：公司未来发展前景不佳

#### 6\. 代理人问题（agency issues）理论

公司管理层和股权人之间

- 管理层可能会过度投资（overinvest）造成不必要的浪费
- 解决办法：增加股利支付率（dividend payout ratio）能缓解这一问题

股权人和债权人之间

- 在公司偿付债务能力减弱的时候，公司的可能会派发大量股利，减少作为抵押的资产总额（asset base）
- 解决方案：通过在债务合约（debt indenture）中的条款（provision），例如：
	- 限制股利支付（restrictions on dividend payment）
	- 要求维持一定水平的资产债务比率（maintenance of certain balance sheet ratios）

<br><br>

## 11\. 影响股利政策的因素（factors affecting dividend policy）

<br><br>

影响股利政策的因素

- 投资机会（investment opportunity）
  - 更多的投资机会，派发的现金股利更少
- 未来盈利的波动性的预期（expected volatility of future earnings）
	- 如果未来盈利的波动性大，公司对于改变股利政策将更加谨慎
- **所得税考虑（tax consideration）**
  - 有额外现金储备并且想要保持金融稳定型的公司可能会使用股票回购而不是股利派发
- 证券发行成本（floatation cost）
  - 证券发行成本越高，股利越低
- 合约及法律限制（contractual and legal restriction）
  - 资本减值法则（impairment of capital rule）：股利派发（dividend paid） < （retained earning）
  - 有时候，债务契约（debt covenants）规定，在支付股利之前，需要达成一定程度的流动比率（liquidity ratio）和利息覆盖率（coverage ratio）

**所得税考虑（tax consideration）**

1. 双重征税制（double-taxation）
2. 分离征税制（split-tax rate system）
3. 转移征税制（tax-imputation system）

**双重征税制（double-taxation）**

- 在公司层面上，无论是否派发股利，都需要交纳企业相应的所得税
- 在股东层面上，股利会被征收股东相应的所得税

**分离征税制（split-tax rate system）**

- 在公司层面上，净收入作为股利派发的部分，相比于作为保留盈余的部分，被征收的税率更低
- 在股东层面上，股利所得作为通常收入项目（ordinary income）征收所得税

**转移征税制（tax-imputation system）**

- 在公司层面上，净收入进行一定程度上的征税
- 在股东层面上
	- 如果股东的税率比公司税率高，则缴纳相当于差额的所得税（pay the difference）
	- 如果股东的税率比公司税率低，则获得相等于差额的抵免额（tax credit），可用于减免其他方式的收入的所得税

<br><br>

## 12\.股利政策（payout policies）的类型

<br><br>

股利政策（payout policies）的类型

1. 稳定股利政策（stable dividend policy）
2. 固定股利支付率（不常见）（constant dividend payout ratio policy）
3. 剩余股利政策（residual dividend policy）

**1\. 稳定股利政策（stable dividend policy）**

- 公司依照未来长期的收益预测，制定出的特定的股利增长率，所以能达到稳定增加的股利派发
- 目标支付率调整模型（target payout adjustment model）
	- 目标股利支付率（expected dividend）= 过往的股利支付率（previous dividend）+ 预计EPS增长率（expected increase in EPS）× 目标股利支付率（target payout ratio）× 调整因素（adjustment factor）
	- 调整因素（adjustment factor）= 1 / 股利政策生效前剩余的年份数（number of years over which the adjustment in dividends will take place）

**2\. 固定股利支付率（不常见）（constant dividend payout ratio policy）**

- 公司每年将派发特定百分比（a specific percentage）的收益作为它的股利
- 股利的额度因此和收益额有直接关系（vary directly with earning）

**3\. 剩余股利政策（residual dividend policy）**

- 股利的额度是基于用于融资资本预算的权益部分的收益剩余（dividends are based on earnings less funds the firm retains  to finance the equity portion of its capital budget）
	- 股利（dividend）= 收益（earning）- 资本预算（capital budget）×（权益（equity）/资产（asset））
	- 没有股利派发的情况：如果权益投资（equity investment）> 收益（earning）
- 该模型基于公司的：
	- 投资机会日程（investment opportunity schedule）
	- 目标资本结构（target capital structure）
	- 可用的外来资本以及融资成本（access to and cost of external capital）

> 此时公司的主要目标是维持相应的资本结构，只有收益超出目标才会派发股利，收益不足时不分红，而且将增发股票

优点：

- 易于公司使用（easy to use）
- 最大化收益对于投资的分配（maximize allocation of earnings to investment）

缺点：

- 股利会因为收入和投资机遇的变化发生波动（fluctuates with investment opportunities and earnings）
- 因为更高的回报预期和更低的估值造成的不确定性（uncertainty cause higher expected return and lower valuation）

长期剩余股利（long-term residual dividend）

- 公司对于其资本预算进行更长期的计划（a longer time frame），以能够提供更加稳定的股利支付（a more steady dividend payout）
- 任何额外的现金流（any excess cash flows）将会以股票回购的形式支付

<br><br>

## 13\. 股利政策：股票回购vs现金股利
股票回购的基本原理（rationales for share repurchase）

- 税收利益（tax advantages）
	- 当股利税率 > 资本利得税率，股票回购存在税收利益
- 为股价提供信号/支持（share price support/signaling）
- 提供灵活性（added flexibility）
	- 和股利不同，股票回购不是一项长期承诺（not a long-term commitment）
	- 管理者对于股票的回购的“市场时机”可酌情选择（have discretion over "market timing"）
- 弥补由于员工的股权带来的股权稀释（offsetting dilution from employee stock option）
- 提高杠杆率（increase financial leverage）
	- 股票回购提高杠杆率
	- 通过减少权益所占的百分比，修改资本结构（modify capital structure）

股利政策的全球趋势（global trends in payout policy）

- 相对于欧洲公司，美国派发股利的公司的比例更低（a lower proportion of U.S. companies pay dividends）
- 全球范围内，支付现金股利的公司的比例呈现下降趋势（the proportion of companies paying cash dividends has trended downwards）
- 相反，进行股票回购的公司的比例呈现上升趋势（the percentage of companies making stock repurchases has been trending upwards）

<br><br>

## 14\. 股利的安全性/持续性（dividend safety）

股利的安全性/持续性（dividend safety）：计量股利以当前支付率持续的可能性的指标（metric used to evaluate the probability of dividends continuing at the current rate for a company）

- 净收入方法（net income method）
	- 股利支付率（dividend payout ratio）= 股利 / 净收入（dividends/net income）
	- 股利备负/覆盖率（dividend coverage ratio）= 净收入 / 股利（net income/dividends）
- 自由现金流方法（free cash flow method）
	- 权益自由现金流备负 / 覆盖率（FCFE coverage ratio）= 权益自由现金流 /（股利 + 股票回购）
