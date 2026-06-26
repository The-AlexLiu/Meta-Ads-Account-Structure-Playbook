# 从零冷启动到稳定结构：Meta Ads 电商账户搭建方法

## 1. 先重新理解“账户结构”

讨论 Meta Ads 结构时，最容易陷入一个误区：把结构理解成 campaign、ad set 和 audience 的排列组合。

比如，有人会问：

- 到底是 CBO 还是 ABO？
- 要不要单独拆兴趣？
- Broad、Lookalike、Retargeting 应该怎么分？
- Advantage+ Shopping 是不是一定比手动 campaign 好？

这些问题都重要，但它们不是问题的第一层。

第一层问题应该是：

> 这个账户有没有给 Meta 足够清晰、足够集中的学习信号？

如果预算被拆进十几个 campaign，Purchase 分散在几十个 ad set 里，每个广告组都拿不到足够转化，Meta 很难稳定学习。即使受众拆得再精细，账户也可能长期停留在学习阶段，表现忽上忽下。

所以我理解的“稳定结构”，不是最复杂的结构，而是最能帮助系统学习的结构。

## 2. 当前更接近共识的方向

结合 Meta 官方 Performance 5、Advantage+ 自动化产品，以及行业投手在近年实操反馈，当前方向可以概括成五句话：

1. 账户结构要简化，不要把预算和事件切碎。
2. 自动化能力要用起来，包括 Advantage+ campaign budget、Advantage+ placements、Advantage+ Audience 或 Advantage+ Sales。
3. 素材要多样化，真正测试不同角度，而不是同一个视频改十个字幕版本。
4. Pixel 和 CAPI 要尽量准确，因为算法需要真实转化信号。
5. 最后要回到业务结果，而不是只看 Meta 后台 ROAS。

对电商账户来说，这些原则最后会落成一个很朴素的结构：

- 一个主力放量 campaign；
- 一个素材测试 campaign；
- 有必要时再加一个再营销 campaign；
- 大促或节点活动单独处理。

这套结构的重点不是“少”，而是每个 campaign 都必须有明确工作。

## 2.1. 受众的角色也变了

现在我不会再把 Meta Ads 的受众策略理解成“找到一个最精准兴趣包”。

受众仍然重要，但它更多承担四个角色：

| 角色 | 说明 |
|---|---|
| 边界 | 地区、语言、合规年龄、自定义受众排除 |
| 提示 | 兴趣、Lookalike、Custom Audience 作为系统起点 |
| 诊断 | 判断某类场景、人群或购买理由是否有反应 |
| 承接 | 访客、ATC、IC、Engagers 等高意向再营销 |

在 Advantage+ Audience 的语境里，很多输入是 suggestions，不是硬定向。也就是说，兴趣、Lookalike 或 Custom Audience 不一定会把广告严格限制在那群人里。真正更像硬边界的是 location、minimum age、language 和 custom audience exclusions 这类 controls。

所以我会把主力放量放在 Broad / Advantage+ Audience 上，把兴趣、Lookalike 和 Custom Audience 当作启动信号、诊断工具和排除规则，而不是把它们拆成一堆长期主力 ad set。

## 3. 冷启动前，先把信号打通

新账户最常见的问题，是还没有确认追踪和站点成交链路，就急着开始测试素材。

如果 Pixel 事件不准，CAPI 去重异常，Purchase 没有正常回传，Meta 学到的东西就是错的。冷启动阶段本来数据就少，如果少量数据还不可靠，后面无论怎么调 campaign 都很难稳定。

投放前至少要检查：

| 模块 | 检查重点 |
|---|---|
| Business Manager | 广告账户、主页、Instagram、支付方式、权限是否正常 |
| Pixel | PageView、ViewContent、AddToCart、InitiateCheckout、Purchase 是否触发 |
| CAPI | 是否有服务端事件，Pixel 与 CAPI 是否去重 |
| Domain | 域名是否验证，Aggregated Event Measurement 是否设置 |
| Catalog | 商品 ID、价格、库存、图片、链接是否正常 |
| UTM | 是否能在 GA4 或后台识别来源、campaign、ad |
| Landing Page | 移动端加载速度、价格、运费、评论、支付、退换政策是否清晰 |

这一步不产生广告结果，但它决定冷启动数据是否可信。

## 4. 第一阶段：用最简单结构测试产品和素材

冷启动阶段不建议一上来搭复杂漏斗。

更稳的方式是：

| 层级 | 推荐设置 |
|---|---|
| Campaign | Sales |
| Budget | CBO 或 Advantage+ Sales |
| Ad set | 1 个 Broad ad set |
| Optimization | Purchase 优先 |
| Placements | Advantage+ placements |
| Ads | 6-10 条差异化素材 |

这里的关键是“差异化素材”。

差异化不是同一个脚本换三个封面，也不是同一张图改五种颜色。真正有价值的测试应该覆盖不同购买动机：

| 素材角度 | 测试目的 |
|---|---|
| 痛点解决 | 用户是否真的在意这个问题 |
| 产品演示 | 用户是否能快速理解产品价值 |
| 社会证明 | 评论、达人、UGC 是否能降低信任成本 |
| Offer 驱动 | 折扣、套装、免邮是否影响决策 |
| 场景人群 | 哪类场景和人群更容易产生购买 |

这个阶段的目标不是马上放量，而是找到账户里第一批能跑出信号的素材。

## 5. 第二阶段：不要把测试和放量混在一起

当账户开始有素材出单后，最容易犯的错误是：继续把所有新素材都塞进同一个 campaign。

短期看这样省事，长期看会有两个问题：

1. 新素材波动会影响主力 campaign 稳定性。
2. 老素材带着历史学习优势，新素材很难获得公平测试机会。

所以当账户有初步赢家后，应该拆出两个角色：

| Campaign | 角色 |
|---|---|
| Evergreen Scale | 放已经验证过的素材，追求稳定 ROAS / CPA |
| Creative Testing | 测新概念、新达人、新视频、新图片 |

测试 campaign 的价值，不是贡献最大 GMV，而是持续给主力 campaign 输送新赢家。

一个健康账户不是靠某一条爆款素材一直撑着，而是有一个持续产生新素材、新角度、新学习的机制。

## 6. 第三阶段：成熟账户的标准结构

当账户已经有稳定 Purchase、素材测试节奏和主力放量 campaign 后，可以进入成熟结构。

成熟结构可以这样配置：

| Campaign | 预算占比 | 说明 |
|---|---:|---|
| ASC / Advantage+ Sales Scale | 50%-70% | 放已验证素材，追求 GMV、ROAS、CPA 稳定 |
| Creative Testing | 20%-30% | 每周测试新概念，筛选下一批 winner |
| Retargeting / DPA | 0%-10% | 只在站点流量和加购量足够时开 |
| Seasonal / Promo | 单独预算 | 大促、节日、清仓、上新，不污染 evergreen 数据 |

这个结构不是固定公式，而是一个决策框架。

如果预算很小，不要强行开再营销。如果国家之间语言、价格、履约差异很大，可以拆地区。如果产品线毛利和客单价差异很大，可以按产品线拆 campaign。

拆分的前提永远是：拆完以后，每个结构仍然有足够预算和转化信号。

## 7. 放量时更应该控制节奏

放量不是简单把预算翻倍。

比较稳的放量方式：

- 主力 campaign 每 3-4 天加 15%-30%；
- 如果短期波动大，先等归因窗口和学习稳定；
- 大促 campaign 单独开，不要把 evergreen campaign 改得面目全非；
- 老素材仍在贡献转化时，不要因为“想保持干净”就过早暂停；
- 新素材通过测试后，再复制到主力 campaign。

判断是否要暂停或调整，可以用下面的规则：

| 情况 | 动作 |
|---|---|
| 单素材花费达到 2 倍目标 CPA，完全无有效行为 | 暂停或换角度 |
| 有 ATC / IC 但无 Purchase | 检查价格、运费、结账、信任背书 |
| CPA 连续 3-5 天高于目标 30%+ | 降预算或回滚最近改动 |
| Frequency 上升、CTR 下降、CPA 上升 | 标记素材疲劳，上新素材 |
| ROAS 下降但 AOV 上升 | 结合毛利、GMV 和回收周期判断 |

## 8. 作品集中的项目表达

这个项目可以这样写进作品集：

> 我将 Meta Ads 账户结构从“多 campaign、多兴趣、多 ad set 的碎片化投放”，重构为“主力放量 + 素材测试 + 可选再营销 + 大促独立”的简化结构。通过集中预算和 Purchase 信号，让 campaign 更容易完成学习；通过独立素材测试机制，让账户持续产生新 winner，避免依赖单条爆款素材导致疲劳。

可展示的产出包括：

- Before / After 账户结构图；
- 冷启动检查清单；
- 素材测试记录表；
- Winner 迁移规则；
- 放量和暂停判断规则；
- Meta、GA4、Shopify 数据口径说明。

这套方法论的重点不是背设置，而是建立一个能持续学习、持续测试、持续放量的广告系统。
