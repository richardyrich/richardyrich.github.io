---
layout: post
title: CFA Level 2 权益 Part 1
categories: CFA2级笔记
---

## 目录
1. 公司价值（valuation）
2. 计算权益风险溢价（equity risk premium）
3. 计算权益要求回报率（required rate of return on equity）
4. 行业分析
5. 策略定制（strategy formation）
6. 绝对价值：现金流折现（discounted cash flow）

<br><br>

## 1\. 公司价值（valuation）

<br><br>

基本概念：

- 内在价值（intrinsic value）
  - 使用正确的估值方法获得的理论价值
- 公允市场价值（fair market value）
  - 主动（willing），信息透明（informed），具有正确判断力（able）的非关联方买家和卖家达成的价格
- 投资价值（investment value）
  - 对于一个特定的买家的价值
- 超额利润（alpha）
  - 事前alpha（ex ante alpha）：预计收益 - 要求收益
  - 时候alpha（ex post alpha）：实际收益 - 应有收益

<br><br>

### 分析的过程（valuation process）

<u>1\. 对行业的认知（understanding the business）</u>

- 行业结构要素（elements of industry structure）（波特五力分析（porter‘s five forces））
  - 新加入的行业竞争者的威胁（threat of new entrants in the industry）
  - 替代者的威胁（threat of substitutes）
  - 买家的议价能力（bargaining power of buyers）
  - 供应商的议价能力（bargaining power of suppliers）
  - 现有竞争者的竞争力（rivalry among existing competitors）
- 两个常见的基本策略（generic strategies）
  - 成本领先战略（cost leadership）
  - 差异化战略（differentiation）

<u>2\. 预测公司业绩（forecasting company performance）</u>

- 自上而下的投资策略（top-down forecasting approach）
- 自下而上的投资策略（bottom-up forecasting approach）
- 对于财务报表的附注进行细节分析（detailed examination of the footnotes accompanying the financial reports）
  - 对于收入的确认过快或过早地确认（accelerating or premature recognition of income）
  - 对于收益和非运营收入的再分级（reclassifying gains and non-operating income）
  - 支出的确认和损失（expense recognition and losses）
  - 表外资产问题（off-balance-sheet issues）（特殊目的实体（special purpose entity），经营租赁（operating lease））

<u>3\. 使用合理的价值模型（selecting the appropriate valuation model）</u>

- 绝对价值模型（absolute valuation model）
  - 股利折现模型（dividend discount model），自由现金流模型（free cash flow)，剩余收益法（residual income approach），基于资产的模型（asset-based model）
- 相对价值模型（relative valuation model）
  - 乘数定价模型（multiple），比如市盈率（P/E）乘数，市净率（P/B）乘数，自由现金流量乘数（P/CF）
- 由预测得出估值（converting forecast to a valuation）
- 做出投资决策（making investment decision）

<br><br>

**分类加总估值法（sum-of-the-parts valuation）**

- 将公司的各部分分开估值，然后再加总
- 多元化折让（conglomerate discount）
  - 默认来说，多元化的经营不如专注经营

多元化折让的原因

- 内部资金的低效使用（internal capital inefficiency）
  - 由于不理想的决策导致资金的消耗
- 内生因素（endogenous (internal) factors）
- 研究测量错误（research measurement errors）
  - 多元化折让来自于分析师测算错误

关于收益（return）的基本概念

- 持有期收益率（holding period return）
  - 完整的投资期限中的收益率
- 实现收益率（realized return）
  - 事后（ex post）的收益率
- 期望收益率（expected return）
  - 事先（ex ante）的收益率
- 要求收益率（required return）（= 机会成本（opportunity cost））
- 内部收益率（internal rate of return）
- 风险溢价
  - 使用资本资产定价模型（capital asset pricing model）计算
  - 使用累加法（build-up approach）计算

> **组合 part 1 也有提及资本资产定价模型（capital asset pricing model）计算**

> - E (R<sub>i</sub>) = R<sub>f</sub> + β (E(R<sub>M</sub>) - R<sub>f</sub>)
> - 是单因子模型，只和系统性风险有关

> **组合 part 2 也有提及使用累加法（build-up approach）计算权益风险溢价：**

> - 权益风险溢价（equity risk premium）：企业的权益的风险溢价
> - 权益收益率 = 无违约无风险利率 + 膨胀率 + 通货膨胀风险溢价 + 权益风险溢价（equity risk premium）
> - 股票对于未来消费的对冲（consumption hedge）能力弱，导致 权益风险溢价 > 信用风险溢价

<br><br>

## 2\. 计算权益风险溢价（equity risk premium）

<br><br>

**计算权益风险溢价的五个方法（宏观的分析，指市场而不是个股）**

<u>1\. 历史型估测（historical estimate）：使用历史数据进行估计</u>

- 权益风险溢价 = 广基权益指数收益率（broad-based equity-market index） - 无风险利率（risk free rate）
- 使用历史数据估计存在的问题
  - 权益指数的代表性：权益指数是否良好反映市场平均水平。广基权益指数一般是市值加权指数（market-value weighted index）
- 缺点：会受到幸存者偏差（survivorship bias）的影响

> 计算股票的溢价时，使用的无风险利率是长期国债的利率，因为股票的假设是长期投资
> 计算衍生品的定价时，使用的是短期国债的利率

<u>2\. 预测型估测（forward-looking estimate）：戈登股利增长模型（gordon growth model）</u>

- = 预测的未来一年市场指数的股利收益率（one year forecasted dividend yield on market index）+ 市场公认的长期增长率（consensus long-term earnings growth rate）- 长期政府债券收益率（long-term government bond yield）
- ERP = r - RFR = D<sub>1</sub> / P<sub>1</sub> + g - RFR
- 假设增长率恒定
- 经济过热状态下（boom），股利收益变低，增长期望变高，分析师需要考虑到这个因素并进行调整


<u>3\. 预测型估测：内部收益率</u>

- 权益指数价格 = PV<sub>rapid</sub>(r) + PV<sub>transition</sub>(r) + PV<sub>mature</sub>(r)

<u>4\. 预测型估测：供应面分析（supply-side estimate）（宏观经济模型）</u>

- = [ ( 1 + i ) × ( 1 + rEg ) × ( 1 + PEg ) - 1 ] + Y -RFR
  - [ ( 1 + i ) × ( 1 + rEg ) × ( 1 + PEg ) - 1 ] 相当于戈登股利增长模型中的D<sub>1</sub> / P<sub>1</sub>，Y相当于g
- i：期望通胀率 = 20年期国债的持有期回报率 - 20年期通货膨胀保值债券（TIPS）
- rEg：期望真实GDP增长率 = 劳动生产率增长（labor productivity growth rate）+ 劳动力增长率（labor supply growth rate）
- PEg：市盈率的变化
- Y：指数的期望回报率

> 在经济 part 2 中涉及到了劳动生产率增长会计法（labor productivity growth accounting equation）

> Y = yL → △Y / Y = △y / y + △L / L
> △y / y：劳动生产率的长期增长率
> △y / y体现了资本深化和科技进步影响

<u>5\. 预测型估测：调研</u>

<br><br>

## 3. 计算权益要求回报率（required rate of return on equity）

<br><br>

**计算权益要求回报率（equity required rate of return）时，分析师可以选择以下五种模型**

1. 资本资产定价模型
2. 多因子模型（multifactor model）
  - 法马-佛伦奇三因子模型（fama-french model）
  - 帕斯托尔-斯坦博模型（pastor-stambaugh model）
  - 宏观经济多因子模型（macroeconomic multifactor model）
3. 累加法（build-up approach）
  - 债券回报率 + 风险溢价

> 组合 part 1 也涉及到了权益要求回报率的相关模型，涉及到的模型和这里有所出入

> - 模型1：资本资产定价模型（capital asset pricing model）
> - 模型2：套利定价模型（arbitrage pricing model）
> - 模型3：多因子模型1 - 宏观经济因子模型（macroeconomic factor model）
> - 模型4：多因子模型2 - 基本面因子模型（fundamental factor model）
> - 模型5：多因子模型3 - 统计因子模型（statistical factor model）

### a）资本资产定价模型

- = 无风险收益率 + β × 权益风险溢价
- 假设：
  - 投资者风险厌恶（risk aversion）
  - 投资者基于马科维茨均值方差结构（markowitz mean-variance framework）进行投资，在相同的波动率下总是偏好最高的收益

估算上市公司的β

- 使用指数：比如标普500或者纽约证券交易所综合指数（NYSE composite）
- 时长 & 频率
  - 一般来说，最近5年的月数据
  - 高速增长领域，最近2年周数据
- 调整后 β（adjusted β）
  - 调整后 β = ( 2 / 3 ) × 未调整 β + ( 1 / 3 ) × 1
  - β 漂移（drift）：长期来看，公司的 β 趋近于1

估算非上市公司的 β

1. 选取可比的基准公司（benchmark company）
2. 估算基准公司的 β
3. 将基准公司的 β 去杠杆（unlever）
  - β<sub>U</sub> ≈ β<sub>E</sub> × ( Equity / Asset )
4. 根据被研究公司的资本结构再杠杆（lever up）
  - β'<sub>E</sub> = β'<sub>U</sub> × ( Asset' / Equity' )
5. 计算结果为被研究公司的 β

### b）法马-佛伦奇三因子模型（fama-french model）

- = RFR + β<sub>mkt, j</sub> × ( R<sub>mkt</sub> - RFR ) + β<sub>SMB, j</sub> × ( R<sub>small</sub> - R<sub>big</sub> ) + β<sub>HML, j</sub> × ( R<sub>HBM</sub> - R<sub>LBM</sub> )

相关参数：

- β<sub>SMB, j</sub>：small market beta
  - 如果β<sub>SMB, j</sub> > 0，该公司为小公司
  - “小公司效应”，小市值公司相对于大市值公司有额外 β
- β<sub>HML, j</sub>：high book-to-market beta，市净率的倒数
  - 如果β<sub>HML, j</sub> > 0，该公司为价值股
  - “价值股表现优于成长股”：高价值公司相对于低价值公司额外 β

### c）帕斯托尔-斯坦博模型（pastor-stambaugh model）

在法马-佛伦奇模型的基础上上加上了流动性 β

- = RFR + β<sub>mkt, j</sub> × ( R<sub>mkt</sub> - RFR ) + β<sub>SMB, j</sub> × ( R<sub>small</sub> - R<sub>big</sub> ) + β<sub>HML, j</sub> × ( R<sub>HBM</sub> - R<sub>LBM</sub> ) + β<sub>i</sub><sup>liq</sup> × ( R<sub>LL</sub> - R<sub>HL</sub> )

相关参数：

- β<sub>i</sub><sup>liq</sup>：liquidity beta
  - 如果β<sub>i</sub><sup>liq</sup> > 0，该公司股票流动性低
  - “流动性溢价”，低流动性要求回报率更高

### d）宏观经济多因子模型（macroeconomic multifactor model）

布尔迈斯特-罗尔-罗斯模型（burmerster roll ross model）包含以下5个因子

1. 信心风险（confidence risk）
  - 风险企业债券和国债之间的利差的异常（surprise）
2. 投资期限风险（time horizon risk）
  - 短期国债和长期国债之间的利差的异常
3. 通货膨胀风险（inflation risk）
  - 通胀率的异常
4. 经济周期风险（business-cycle risk）
  - 商业活动的异常
5. 市场时机风险（market timing risk）
  - 任何前四个无法解释的因素

### e）累加法（build-up approach）

权益收益的基本概念

- = RFR + 权益风险溢价 ± 其他溢价

对于非上市公司（private business）的价值

- = RFR + 权益风险溢价 + 规模溢价（size premium）+ 公司相关的溢价（specific-company premium）

债券收益加风险溢价法（bond yield plus risk premium method）

- = 公司长期债券的持有期收益率 + 风险溢价

<br><br>

**国际考虑（international consideration）**

- = 权益风险溢价 = 发达国家的权益风险溢价 + 国家溢价（country premium）

国家利差模型（country spread model）：使用相对应的发达国家市场作为基准，并加入发展中国家的溢价

- 溢价为两个市场之间的债权收益率利差

**加权平均资本成本（weighted average cost of capital (WACC)）**

- 债券应该使用市场价值而不是账面价值
- 债券融资成本应该考虑税收影响

要求回报率（=折现率，机会成本）

- 权益自由现金流量（cash flow to equity）使用的折现率：权益的要求回报率
- 公司自由现金流（cash flow to the firm）使用的折现率：公司的融资成本（税后加权平均资本成本）

现金流的金额可以使用名义（nominal）现金流或者真实（real）现金流

- 名义现金流：使用名义折现率
- 真实现金流：使用真实折现率
- 计算出的结果其实是一样的

<br><br>

## 4\. 行业分析

<br><br>

使用的是自上而下的投资策略（top-down forecasting approach）

行业分析

- 行业吸引力（industry attractiveness）：行业在长期以来是否有收益潜力
- 行业竞争力（competitive advantage）：公司将如何给买家创造价值，相对于其他公司能做的多好

**波特五力分析**

<u>1\. 新加入的行业竞争者的威胁（threat of new entrants in the industry）</u>

- 规模经济（economies of scale）
- 产品差异和品牌特性（product differences and brand identity）
- 消费者的转换成本（switching cost）
  - 消费者的转换成本越低，对新进竞争者越有利
- 资本需求（capital requirement）
  - 进入行业需要初始花费
- 分销网络（access to distribution channels）
  - 容易建立分销网络更利于新竞争者
- 政府政策
- 成本或者质量的优势

<u>2\. 替代品（substitute product）</u>

- 替代品的相对性价比（relative price performance）
- 买家替换的意愿（propensity to substitute）
- 转换成本

差异化产品更难被替代

<u>3\. 买家的议价能力（bargaining power of buyers）</u>

- 谈判杠杆（bargaining leverage）
  - = 谈判能力
  - 比如低转换成本，或者替代品是否方便获得（readily available）
- 价格敏感性（price sensitivity）

<u>4\. 供应商的议价能力（bargaining power of suppliers）</u>

- 原材料的差异性（differentiation of input）
- 原材料的替代品是否存在
- 供应商的垄断程度（concentration）
- 向前整合（forward integration）的威胁
  - 产业链向消费者方向进行整合
- 转换成本

<u>5\. 现有竞争者的竞争力（rivalry among existing competitors）</u>

- 竞争者的数量
- 行业增长率
- 高度运营和金融杠杆（operating or financial leverage）
- 参与者的投入性（participant's commitment）
- 产品差异性
- 产品的生命周期（shelf life）
- 退出障碍（exit barrier）
- 信息的复杂度（informational complexity）

**长期影响因素**

（波特五力分析主要的重心是短期因素）

- 行业增长率
- 科技和创新
- 政府政策
- 互补产品（complementary product）

<br><br>

## 5\. 策略定制（strategy formation）

<br><br>

评估行业的因素

- 可预见性（predictability）
  - 行业需求
  - 公司表现
  - 市场预期
- 可变性（malleability (mutability)）
  - 公司和其竞争者是否能影响这些行业因素

<br><br>

**策略的类型（strategy formation style）**

<u>1\. 传统型（classical）策略的特点：</u>

- 高度可预见（highly predictable）
- 行业的参与公司不容易轻易改变市场特征
- 例子：石油行业

策略

1. 需要确定公司具体的独特竞争能力和资源
2. 设定计划
3. 计划的目标之一：效率优化（optimize efficiency）
4. 适用波特五力分析

<u>2\. 适应型（adaptive）策略的特点：</u>

- 高度不可预测
- 行业的参与公司不容易改变市场特征
- 例子：特殊时装零售(specialty fashion retailing)

策略

1. 需要依照环境持续调整长期目标
2. 快速再分配（redistribute）和获取（acquire）资源
3. 计划的目标之一：灵活性（flexibility）
4. 短期目标多为猜测而非确凿计划
5. 目标主要围绕（closely linked to）运营过程（operation process）而展开

<u>3\. 成形型（shaping）策略的特点：</u>

- 不可预测
- 行业可被改变
- 例子：软件行业

策略

1. 较短的计划周期，高度灵活性
2. 创造行业影响力（seek to influencec the unpredictable business environment）
  - 建造顾客，供应商，商业伙伴的网络（network）
  - 定义新市场，科技，和商业惯例（practice）
  - 通过营销（marketing），游说（lobbying），策略伙伴（strategic partnership）激发（promote）市场的兴趣

<u>4\. 远景型（visionary）策略的特点：</u>

- 不可预测
- 行业可被改变
- 例子：新创造出的市场

策略

1. 改变环境以便于公司发展
2. 高风险，高破坏性（disruptive），“守株待兔”的策略（"build it and they will come" approach）
3. 条件：
  - 足够的资源
  - 注意力放在长期发展上

<br><br>

计划策略时的常见错误（pitfalls）

- 假设行业总是可以被预测，所以只考虑传统型和远景型策略
- 低估行业的变化速度
- 企业文化不支持企业的策略
- 在不同的领域中单一地使用一个策略

<br><br>

## 6\. 绝对估值法：现金流折现（discounted cash flow）

<br><br>

### a）预测行业增长率

行业增长率相对于GDP的增长率（有两种假设的方式）

- 【加法】比GDP的增长率高x个百分点：g<sub>GDP</sub> + x %
- 【乘法】比GDP的增长率的x %倍：g<sub>GDP</sub> × ( 1 + x % )

### b）预测现金流量表相关科目

<u>1\. 市场增长和市场份额（market share）</u>

- 估算行业销售额（市场增长率）
- 估算公司的市场份额
- 公司销售额 = 行业销售额 × 市场份额
- 需要注意不同地域之间的，GDP增长率和收入增长率的关系可能会有区别

规模经济（economies of scale）

- 当生产量增加时，有更高的边际营业利润（operating margin）
- 销售量和边际利润会呈现正相关性（positively correlated）

<u>2\. 预测主营业务支出（cost of goods sold）</u>

- 和竞争公司的数据进行对比
- 分析公司的投入支出（input cost）

<u>3\. 销售成本、综合开销及行政管理费（selling, general and administrative expenses）</u>

- 固定部分（fixed component）：
  - 研究和开发支出（R&D expenditure）
  - 总部的支出（headquarters expense），管理层薪酬（management salaries），信息技术运营（information technology operation）
- 变动部分（variable component）：
  - 和销售额相关的，比如营销和分销支出（selling and distribution cost）

<u>4\. 融资成本（financing cost）</u>

净贷款额（net debt）

- = 总贷款额 - （货币资金（cash） + 约当现金（cash equivalents）- 短期证券（short-term securities））

净利息支出（gross interest expense）

- = 利息支出- 收入

分析师应该考虑公司的发债和偿债计划，以及公司现有债务的期限结构

<u>5\. 融资成本（financing cost）</u>

分析时需要考虑三种不同的所得税费用（tax expense）

- 法定税率（statutory rate）
- 实际税率（effective tax rate）
- 现金支付税率（cash tax rate）
  - = 现金流量表中的所得税费用 / 利润表中的税前利润

<u>6\. 所得税支出（tax expense）</u>

- = 现金应交税金（cash tax due）+ △递延所得税负债（△ deferred tax liabilities）- △递延所得税资产（△ deferred tax assets）

法定税率&实际税率的差异

- 利润表的有些支出不能抵税
- 两者的对账（reconciliation）会在附注中披露
- 跨国经营公司的实际税率是各国实际税率的加权平均

分析师应留意是否存在实际税率持续地，显著地，比法定税率低的情况

（下部分续）
