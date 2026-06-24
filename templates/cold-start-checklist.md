# Meta Ads 冷启动检查清单

适用时间：新账户上线前，或旧账户重构前。

## 1. 账户与权限

| 检查项 | 状态 | 备注 |
|---|---|---|
| Business Manager 可正常访问 | 待检查 |  |
| 广告账户无风控、无支付异常 | 待检查 |  |
| Facebook Page 已绑定 | 待检查 |  |
| Instagram Account 已绑定 | 待检查 |  |
| Pixel 已分配给广告账户 | 待检查 |  |
| Catalog 已分配给广告账户 | 待检查 |  |

## 2. Pixel / CAPI / Domain

| 检查项 | 状态 | 备注 |
|---|---|---|
| PageView 正常触发 | 待检查 |  |
| ViewContent 正常触发 | 待检查 |  |
| AddToCart 正常触发 | 待检查 |  |
| InitiateCheckout 正常触发 | 待检查 |  |
| Purchase 正常触发 | 待检查 |  |
| CAPI 有服务端事件 | 待检查 |  |
| Pixel 与 CAPI 去重正常 | 待检查 |  |
| Domain 已验证 | 待检查 |  |
| Purchase 事件优先级最高 | 待检查 |  |

## 3. 商品与落地页

| 检查项 | 状态 | 备注 |
|---|---|---|
| 商品链接可正常打开 | 待检查 |  |
| 移动端首屏加载正常 | 待检查 |  |
| 价格、折扣、运费清晰 | 待检查 |  |
| 评论、信任背书、退换政策完整 | 待检查 |  |
| 加购流程正常 | 待检查 |  |
| 结账流程正常 | 待检查 |  |
| 支付方式可用 | 待检查 |  |

## 4. UTM

推荐模板：

```text
utm_source=facebook&utm_medium=cpm&utm_campaign={{campaign.name}}&utm_content={{ad.name}}
```

检查项：

| 检查项 | 状态 | 备注 |
|---|---|---|
| URL 没有多个问号 | 待检查 |  |
| UTM 参数没有重复 | 待检查 |  |
| 没有中文符号或空格 | 待检查 |  |
| `{{campaign.name}}` 和 `{{ad.name}}` 未被错误转义 | 待检查 |  |
| GA4 能识别来源和 campaign | 待检查 |  |

## 5. 第一轮冷启动 Campaign

| 设置项 | 建议 |
|---|---|
| Objective | Sales |
| Optimization | Purchase 优先 |
| Budget | 日预算至少接近目标 CPA 的 3-5 倍 |
| Audience | Broad，只限制国家、语言、合规年龄 |
| Placements | Advantage+ placements |
| Ads | 6-10 条不同角度素材 |
| 判断周期 | 3-7 天，不频繁编辑 |

