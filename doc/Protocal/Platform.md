# 平台

## 建造工程 Masonry (Boardroom)

- 周期时间：6 小时
- 从建造工程中 提取 / 存入 TSHARE 将会导致 TSHARE 被锁定 6 个周期，TOMB 奖励将会被锁定 3 个周期
- 提取 TOMB 奖励会锁定 TSHARE 6 个周期，且在 3 个周期后才能提取第二次 TOMB 奖励
- 膨胀期间的 TOMB 分配：

  **80%** 奖励给予董事会 TSHARE 质押者

  **18%** 给予 DAO 基金

  **2%** 给予 DEV 基金

- 周期膨胀：目前的扩张上限以 TOMB 供应为基础，如果有债券需要赎回，TOMB 铸造的 65% 将归入金库直至解决所有债券赎回需求。如果没有债务，它将遵循最大扩充率。

![Tomb.expansion_v2.png](https://gblobscdn.gitbook.com/assets%2F-MZTnQlB3bvER734QSzS%2F-McWIgfaRAb47_V1r4jh%2F-McWIsY-Ghi63GwQheV2%2FTomb.expansion%20v2.png?alt=media&token=328bec73-2eae-49e6-9465-8d3f36b5c5af)

### Masonry UI 现有信息

下一个 **Seigniorage** 展示了距离下个周期的倒计时（每个周期持续 6 小时）

**APR** 展示了拥有的 TSHARE 的现实价值，单位为美元

_注意：APR 会根据不同原因而不时变动，如以下：_

- TOMB 价值
- TSHARE 价值
- 质押于建造工程（Masonry）的 TSHARE 数量（已锁价值）

### 膨胀期下的建造工程

当 TWAP < 1 时，建造工程**不会**铸造任何 TOMB (没有奖励)

### 债务期下的建造工程

收缩期后的扩张时期仍有 TBonds 需要赎回，此阶段称为债务阶段。

65% 的供应扩张会於债务期时传送回金库以用来准备赎回 TBOND。这金额会被预留，不管 TBOND 持有人会不会赎回 TBOND。

当金库中的 TOMB 足够完全赎回所以流动中的债券後，扩张率会回复正常。

收缩期下每周期排放的 TBOND 可以到规章查看。

---

## 墓地 (股份)

质押你的 LP 获得 TSHARE 代币

LP 池 (股份奖励) 开放 12 个月：

- TOMB-FTM LP: 35500 股
- TSHARE-FTM LP: 24000 股

---

## 矿井 (债券)

当 TOMB 低於 1 FTM 时，TBOND (债券代币)开放买入。

例子：TOMB 的 TWAP < 1，TOMB 能够以 1:1 比例兑换 TBOND。

当 TOMB 高於 1 FTM 时，TBOND (债券代币)开放赎回。

为了鼓励在 TOMB 的 TWAP > 1.1 时用 TBOND 赎回 TOMB，并激励用户以更高的价格赎回 TOMB，在 TOMB 的 TWAP 值较高的情况下，TBOND 赎回将更有利可图，其中 TBOND 与 TOMB 的比例为 1 : R，其中 R 可以用下图的公式计算：

R=1+[(TOMB(twapprice)−1)∗coeff)]

coeff = 0.7
