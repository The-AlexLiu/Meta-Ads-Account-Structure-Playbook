# Meta Ads 账户结构画布

用于梳理一个账户是否需要拆 campaign，以及每个 campaign 的职责是否清晰。

## 1. 业务基础

| 字段 | 内容 |
|---|---|
| 品类 |  |
| 主推产品 |  |
| AOV |  |
| 毛利率 |  |
| 目标 CPA |  |
| 目标 ROAS |  |
| 日预算 |  |
| 主要国家 |  |
| 主要语言 |  |
| 履约时效 |  |

## 2. 当前结构

| Campaign | Objective | Budget | Ad sets | Ads | 主要问题 |
|---|---|---:|---:|---:|---|
|  |  |  |  |  |  |

## 3. 推荐结构

| Campaign | 角色 | 预算占比 | 放什么素材 | 判断指标 |
|---|---|---:|---|---|
| Evergreen Scale | 主力放量 | 50%-70% | 已验证 winner | CPA / ROAS / Purchase / GMV |
| Creative Testing | 素材测试 | 20%-30% | 新概念、新达人、新视频、新图片 | Spend / CPA / CTR / CVR / Hook |
| Retargeting | 高意向承接 | 0%-10% | 评论、保障、offer、DPA | Frequency / CPA / ROAS |
| Seasonal | 大促节点 | 单独预算 | 节日、折扣、清仓、上新 | GMV / CPA / ROAS / 库存 |

## 4. 拆分判断

| 是否需要拆分 | 判断标准 | 结论 |
|---|---|---|
| 按国家拆 | 语言、价格、购买力、履约是否明显不同 | 待判断 |
| 按产品拆 | 产品线、毛利、AOV、落地页是否明显不同 | 待判断 |
| 按 offer 拆 | 折扣、套装、免邮、赠品是否是独立策略 | 待判断 |
| 按受众拆 | 是否有明确证据证明受众差异带来稳定收益 | 待判断 |

## 5. Winner 迁移规则

| 条件 | 动作 |
|---|---|
| CPA 达标且 Purchase 稳定 | 复制到 Evergreen Scale |
| ROAS 达标但样本少 | 保留观察，继续跑到足够花费 |
| CTR 高但无 Purchase | 检查落地页、价格、结账 |
| CPM 高、CTR 低 | 重做 hook 或素材角度 |
| 老素材 Frequency 上升且 CPA 恶化 | 标记疲劳，准备替换 |

## 6. 受众策略检查

| 受众项 | 当前设置 | 判断 |
|---|---|---|
| 主力放量受众 |  | 是否以 Broad / Advantage+ Audience 为主 |
| Audience controls |  | 地区、语言、最低年龄、必要排除是否清楚 |
| Audience suggestions |  | 兴趣、Lookalike、Custom Audience 是否只是辅助信号 |
| Retargeting |  | 流量池是否足够，是否有频次和增量判断 |
| Exclusions |  | 是否排除了不该投的人，又没有过度排除 |
| Audience split |  | 是否因为拆受众导致预算和学习事件被切碎 |
