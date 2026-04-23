# 收单术语表（Glossary）

> 版本：v0.1  
> 更新时间：2026-04-20

## 核心角色

- `持卡人（Cardholder）`：发起支付的一方。
- `商户（Merchant）`：提供商品/服务并接收付款的一方。
- `收单机构（Acquirer）`：为商户提供收单服务并承担收单风险的机构。
- `发卡行（Issuer）`：向持卡人发行银行卡并进行授权决策的机构。
- `卡组织（Card Network）`：定义网络规则并承载成员机构间交易与清结算网络。

## 接入与产品形态

- `支付服务商（Payment Service Provider, PSP）`：聚合多通道能力，为商户提供统一支付接入。
- `支付促进商（Payment Facilitator, PF）`：在赞助收单行体系下为子商户提供聚合收单。
- `支付网关（Payment Gateway）`：负责交易数据采集、加密与路由，不直接持有清算主体资格。
- `支付编排（Payment Orchestration）`：对多 PSP/Acquirer/LPM 的统一路由与策略编排能力。

## 交易生命周期

- `授权（Authorization）`：判断交易是否被允许发生。
- `清算（Clearing）`：确认交易账务事实并形成机构间应收应付。
- `结算（Settlement）`：机构间与机构对商户的资金交收过程。
- `撤销（Void）`：在请款前取消交易，通常不发生正式清算。
- `退款（Refund）`：原交易成功后发起的反向资金流程。

## 风险与争议

- `拒付（Chargeback）`：发卡侧或持卡侧发起的争议扣款流程。
- `第一方欺诈（First-party Fraud）`：真实持卡人发起交易后否认交易或利用规则套利。
- `拒付率（Chargeback Rate）`：争议管理中的关键风险指标。
- `准备金（Reserve）`：针对风险敞口预留的商户资金。
- `KYC（Know Your Customer）`：客户身份识别与尽职调查。
- `AML（Anti-Money Laundering）`：反洗钱管理体系。
- `PCI DSS（Payment Card Industry Data Security Standard）`：卡数据安全标准。
- `3DS（3-D Secure）`：卡支付认证协议，常用于电商交易认证。
- `SCA（Strong Customer Authentication）`：强客户认证要求，强调多因子认证。
- `TRA（Transaction Risk Analysis）`：基于风险评分的认证豁免策略。
- `MIT（Merchant Initiated Transaction）`：商户发起交易，如续费、分期后续扣款。
- `RDR（Rapid Dispute Resolution）`：快速争议解决机制，通常在正式拒付前处理。
- `Ethoca Alerts`：争议预警服务，帮助商户在拒付前处置风险交易。

## 货币与账务

- `交易币种（Transaction Currency）`：消费者支付时的币种。
- `清算币种（Clearing Currency）`：网络/成员清算时采用的币种。
- `结算币种（Settlement Currency）`：商户最终到账币种。
- `净额结算（Net Settlement）`：汇总多笔应收应付后按净额交收。
- `对账（Reconciliation）`：跨系统核对交易、账务、资金一致性的过程。
- `编排（Orchestration）`：将分流、规则、任务、提交等流程自动串联并可回滚的能力。
- `数据驻留（Data Residency）`：数据必须在指定司法辖区内存储与处理的要求。
- `跨境传输（Cross-border Data Transfer）`：数据在不同司法辖区间传输的合规过程。
- `制裁筛查（Sanctions Screening）`：对交易主体进行制裁名单核验的控制动作。
- `Runbook`：标准化故障处置步骤清单，可人工或自动执行。
- `MTTA（Mean Time to Acknowledge）`：平均响应时间。
- `MTTR（Mean Time to Recovery）`：平均恢复时间。
- `值班（On-call）`：按班次负责告警响应与故障处置的机制。
