# 独立服务器：RackNerd 全系 23 款套餐价格对比，附终身 85 折优惠码与退款避坑指南

租独立服务器最怕两件事：花了大价钱拿到手发现配置名不副实，或者买完才发现根本不退款。这篇文章把 RackNerd 目前在售的全部独立服务器套餐（Hybrid 混合独服、Xeon 裸金属、Ryzen 裸金属、10Gbps 不限流量四条线，共 23 款）的配置和价格整理成表，算清用官方优惠码 15OFFDEDI 之后的真实月成本，再把退款政策里藏在条款里、但直接影响下单决策的几条限制提前讲清楚。

先说结论：RackNerd 的独服门槛在 $39/月（Hybrid 4GB），真正意义上的裸金属从 $139/月起步；所有独服结账时输入优惠码 **15OFFDEDI** 可以终身 85 折，折后裸金属入门约 $118/月。适合需要独享硬件、root 权限、大流量配额的用户。

> **选购速览**：大多数只需要“一台性能有保障的整机器”的读者，选入门裸金属 E3-1230 v2（16GB/480GB SSD/35TB 流量/5 个 IP），原价 $139/月，用 15OFFDEDI 后约 **$118.15/月**，结账时在促销码栏填入即可。预算紧、要快速开通的，Hybrid 4GB（$39/月）够用。👉 [查看 RackNerd 独立服务器全部套餐与当前价格](https://bit.ly/RacKnerd)

## RackNerd 的独立服务器分四条线，先搞清楚区别

四条线的核心差异在于“是不是整机、什么 CPU、什么端口”。买错产品线的代价不小，比如想要洛杉矶低延迟却下单了 Ryzen——Ryzen 线目前只在犹他州部署。

- **Hybrid 混合独服**（$39–$99/月）：部署在一台双路 Xeon E5-2690 2.90GHz 的物理机上，你独占分配到的 CPU 核心和内存，存储是 HDD。优势是**即时开通**，价格最低，内置 10Gbps DDoS 防护。劣势是存储全是机械盘，磁盘 IO 是明显瓶颈。
- **Bare Metal Intel Xeon 裸金属**（$139–$479/月）：整台物理机，含 IPMI/KVM 控制台、远程重启，支持 Linux、Windows、FreeBSD 和自定义 ISO，官方口径 48 小时内交付。1Gbps 端口，流量 35TB 到 200TB 不等，多数配置含 5 个 IPv4。
- **AMD Ryzen 裸金属**（$219–$499/月）：DDR5 + NVMe 新平台，单核性能远强于同价位 Xeon 老款，多数当天部署，40TB 流量 @ 1Gbps，只带 1 个 IP。**目前仅犹他州数据中心**，官方表示后续会增加位置。需要洛杉矶或纽约低延迟的，只能选 Xeon 线或邮件联系 sales 定制。
- **10Gbps 不限流量裸金属**（$599–$1,999/月）：端口固定 10Gbps，无月流量上限、不按 TB 计费、无超额费用，可选洛杉矶、新泽西、伦敦、蒙特利尔，均含 5 个 IPv4。

## 全套餐价格表（含折后参考价）

以下价格均为官网月付原价（美元）。“折后”一列按 15OFFDEDI（85 折）计算。两条裸金属线先看这张主表：

**Hybrid 混合独服 + Bare Metal Xeon 裸金属（1Gbps 端口）**

| 套餐 | 核心配置 | 流量 | IPv4 | 月付原价 | 购买 |
| --- | --- | --- | --- | --- | --- |
| Hybrid 4GB | 双 E5-2690 / 2 核 / 4GB / 120GB HDD | 5TB | 1 个 | $39 | [订购 Hybrid 4GB](https://my.racknerd.com/aff.php?aff=11397&pid=4) |
| Hybrid 8GB | 4 核 / 8GB / 250GB HDD | 5TB | 1 个 | $59 | [订购 Hybrid 8GB](https://my.racknerd.com/aff.php?aff=11397&pid=5) |
| Hybrid 16GB | 6 核 / 16GB / 500GB HDD | 10TB | 1 个 | $79 | [订购 Hybrid 16GB](https://my.racknerd.com/aff.php?aff=11397&pid=6) |
| Hybrid 32GB | 8 核 / 32GB / 750GB HDD | 10TB | 1 个 | $99 | [订购 Hybrid 32GB](https://my.racknerd.com/aff.php?aff=11397&pid=7) |
| Entry Xeon | Xeon E3-1230 v2 / 16GB / 480GB SSD | 35TB | 5 个 | $139 | [订购 Entry Xeon](https://my.racknerd.com/aff.php?aff=11397&pid=12) |
| Mid Xeon | Xeon E3-1270 v3 / 32GB / 2×1TB SSD | 35TB | 5 个 | $169 | [订购 Mid Xeon](https://my.racknerd.com/aff.php?aff=11397&pid=869) |
| Dual E5 Base | 双路 E5-2650 v2 / 64GB / 1TB SSD | 100TB | 5 个 | $199 | [订购 Dual E5 Base](https://my.racknerd.com/aff.php?aff=11397&pid=867) |
| Dual E5 + HDD | 双路 E5-2650 v2 / 128GB / 1TB SSD+3TB HDD | 50TB | 5 个 | $245 | [订购 Dual E5 + HDD](https://my.racknerd.com/aff.php?aff=11397&pid=871) |
| Virtualization Node | 双路 E5-2650 v2 / 256GB / 4×2TB SSD | 100TB | 29 个 | $349 | [订购 Virtualization Node](https://my.racknerd.com/aff.php?aff=11397&pid=868) |
| Dual E5-2680 v4 | 双路 E5-2680 v4 / 256GB / 4×2TB SSD | 100TB | 61 个 | $399 | [订购 Dual E5-2680 v4](https://my.racknerd.com/aff.php?aff=11397&pid=870) |
| 160TB Storage Special | 双路 E5-2640 v2 / 64GB / 256GB SSD+10×16TB HDD | 200TB | 5 个 | $479 | [订购 Storage Special](https://my.racknerd.com/aff.php?aff=11397&pid=526) |

Storage Special 位于洛杉矶 DC-02，10 块 16TB 机械盘加 160TB 月流量，明显是给备份池、媒体归档、下载站这类大容量场景准备的。Virtualization Node 和 E5-2680 v4 分别给 29 个和 61 个 IPv4，是全系里 IP 数量最高的两款，适合打算开 VPS 或跑多站点业务的人。

**AMD Ryzen 裸金属（40TB @ 1Gbps，1 个 IPv4，仅犹他州）**

| 套餐 | 配置 | PassMark | 月付原价 | 购买 |
| --- | --- | --- | --- | --- |
| Ryzen 5 7600 | 64GB DDR5 / 1TB NVMe | 27,109 | $219 | [订购 Ryzen 5 7600](https://my.racknerd.com/aff.php?aff=11397&pid=861) |
| Ryzen 7 7700 | 64GB DDR5 / 1TB NVMe | 34,536 | $249 | [订购 Ryzen 7 7700](https://my.racknerd.com/aff.php?aff=11397&pid=862) |
| Ryzen 9 7900 | 64GB DDR5 / 1TB NVMe | 48,825 | $269 | [订购 Ryzen 9 7900](https://my.racknerd.com/aff.php?aff=11397&pid=864) |
| Ryzen 9 5950X（限时） | 128GB DDR4 / 2TB NVMe | — | $309 | [订购 5950X 限时款](https://my.racknerd.com/aff.php?aff=11397&pid=863) |
| Ryzen 9 7950X3D | 128GB DDR5 / 1TB NVMe | 62,433 | $379 | [订购 7950X3D 128GB](https://my.racknerd.com/aff.php?aff=11397&pid=865) |
| Ryzen 9 7950X3D | 192GB DDR5 / 2×3.84TB NVMe | — | $499 | [订购 7950X3D 192GB](https://my.racknerd.com/aff.php?aff=11397&pid=866) |

同一预算下，Ryzen 的 PassMark 分数几乎是 Xeon 线的两倍以上：$269 的 Ryzen 9 7900 跑到 48,825 分，而 $349 的 Virtualization Node 用的双路 E5-2650 v2 合计 PassMark 约 17,275 分——这款 2013 年三季度上市的处理器，单线程分数只有 1,661，面对 Ryzen 7900（单核分数高出两倍多）毫无还手之力。单核性能敏感的应用（游戏服、编译、实时处理）在 Ryzen 上每块钱换到的算力明显更多。反过来说，E5-2650 v2 的多线程性价比（CPU Mark/$Price 66.47）在服务器 CPU 里并不算差，批量跑虚拟机、跑对单核不敏感的并行任务，它依然能用。

**10Gbps 不限流量裸金属（5 个 IPv4，可选洛杉矶/新泽西/伦敦/蒙特利尔）**

| 套餐 | 配置 | 月付原价 | 购买 |
| --- | --- | --- | --- |
| Entry Special（限时） | Xeon E3-1230 V3 / 32GB DDR3 / 1TB SSD | $599 | [订购 10Gbps 入门款](https://my.racknerd.com/aff.php?aff=11397&pid=746) |
| Xeon E-2136 | 6C/12T / 32GB DDR4 / 1TB NVMe | $799 | [订购 E-2136](https://my.racknerd.com/aff.php?aff=11397&pid=747) |
| Dual E5-2630 V4 | 20C/40T / 64GB DDR4 / 1TB NVMe | $950 | [订购 Dual E5-2630 V4](https://my.racknerd.com/aff.php?aff=11397&pid=748) |
| Dual E5-2695 V4 | 36C/72T / 128GB DDR4 / 2×1TB NVMe | $1,399 | [订购 Dual E5-2695 V4](https://my.racknerd.com/aff.php?aff=11397&pid=749) |
| EPYC 7642 | 48C/96T / 128GB DDR4 / 2×1TB NVMe | $1,699 | [订购 EPYC 7642](https://my.racknerd.com/aff.php?aff=11397&pid=750) |
| EPYC 7702P | 64C/128T / 128GB DDR4 / 2×1TB NVMe | $1,999 | [订购 EPYC 7702P](https://my.racknerd.com/aff.php?aff=11397&pid=751) |

$599 入门款在官网被标注为限时特价，库存清完可能下架；它用的 E3-1230 V3 是 Haswell 时代的老 CPU，但带宽型负载（CDN 源站、静态文件镜像）下单个 nginx 进程就能吃满 10Gbps，瓶颈根本轮不到 CPU。要跑转码、容器集群这类吃算力的活，再加两百块上 $799 的 E-2136 更合理。

## 15OFFDEDI 优惠码：续费也是 85 折，这点和多数主机商不一样

15OFFDEDI 是 RackNerd 官方长期公开的独服优惠码，覆盖全部独立服务器（包括 10Gbps 系列），折扣力度 15%，**循环生效、终身有效**——每张账单都减 15%，续费同样打折，只针对首月或首年的促销码完全不是一个概念。

使用方式：结账页面的促销码栏填入 15OFFDEDI，折扣立即生效。折后的真实月成本大致如下：

- Hybrid 4GB：$39 → **$33.15/月**
- Entry Xeon 裸金属：$139 → **$118.15/月**
- Ryzen 9 7900：$269 → **$228.65/月**
- Dual E5-2680 v4：$399 → **$339.15/月**
- 10Gbps EPYC 7702P：$1,999 → **$1,699.15/月**

按年算，Entry Xeon 折后一年约 $1,417.80，比原价 $1,668 省下约 $250。没有复杂的叠加规则，也不用凑活动周期，什么时候下单折扣都在。👉 [用优惠码 15OFFDEDI 开通 Entry Xeon 裸金属](https://my.racknerd.com/aff.php?aff=11397&pid=12)

## 退款政策：默认不退款，下单前把这两件事做完

RackNerd **没有退款保证（money back guarantee）**。官方服务条款的原话是：付款后默认不提供退款，退款按个案酌情处理。没有 7 天或 14 天的无理由退款窗口，预充值到账户的余额也明确不能退。这是它低价模式的一部分，下单前必须知道。

能争取到退款的情形很窄：服务刚开通几分钟就发现明显异常（起不来、IP 不通）、独立服务器超过 72 小时未交付（官方承诺 72 小时内交付）、存在明确技术故障且尚无实际使用记录。已经被使用过一段时间、或纯粹是个人需求变更的，大概率被拒。被拒时客服常见的替代方案是转成账户余额、换机房位置或换更高配置补差价。

另外两条容易被忽略的规则：

- 点了“立即取消”后系统 24 小时内终止服务，**所有数据立即删除且不可恢复**。取消和退款是两回事：取消只停后续续订，不返还已付费用。
- 直接对信用卡发起拒付（chargeback）会触发 **$125–$250 的行政费**，账户还可能被暂停。

因为默认不退款，降低风险的办法要在下单前做：RackNerd 每个机房都提供 Looking Glass 测试工具，有公开的 test IP 和 100MB/1GB 测试文件，下单前先跑 ping 和 traceroute 确认到你本地的线路质量。独服用户还想再稳妥一点，可以先开一台月付的 Hybrid 或廉价 VPS 试一两个月线路，再上裸金属。👉 [先测线路，再看全部套餐配置](https://bit.ly/RacKnerd)

## 按场景选套餐：一张决策清单

- **低流量工具节点（邮件中继、监控、面板）**：Hybrid 4GB，$39/月。HDD 是硬伤，别碰数据库。
- **小型 SaaS、staging 环境**：Hybrid 16GB（$79/月）能跑小型 Postgres + Node 应用；要 SSD 就直接上 Entry Xeon。
- **自托管 GitLab、中流量 WordPress 多站、需要稳定 IO 的 CI runner**：Entry Xeon，折后 $118/月，带 IPMI 的真裸金属。
- **游戏服、编译农场、实时处理（单核性能敏感）**：Ryzen 线，$219 起步，接受它只有犹他州一个位置、1 个 IP。
- **自建 VPS 出售或多 IP 业务**：Virtualization Node（29 IP，$349/月）或 Dual E5-2680 v4（61 IP，$399/月）。
- **备份池、媒体归档、下载站**：160TB Storage Special，$479/月，洛杉矶 DC-02。
- **CDN 源站、直播推流、大文件镜像（带宽敏感）**：10Gbps 系列，$599 入门款先用着，算力不够再升 $799 的 E-2136。

## 下单前的最后确认

三条短提醒，都在付款按钮之前完成：

1. **线路先测再买**。用目标机房的 Looking Glass 和 test IP 跑一遍 ping、traceroute、MTR，特别是晚高峰时段。退款没保障，线路不合预期就只能靠客服协商换机房。
2. **数据自己管**。所有独服默认非托管、不含备份，RackNerd 声明不对数据完整性负责；逾期 3 天未续费，服务器就可能被释放，数据随之清除。装好系统的第一件事是搭异地自动备份。
3. **月付试水，年付锁定**。新机房、新线路先按月付开一台跑满一个月，确认稳定再考虑长期；下单时记得填 15OFFDEDI，这个码续费同样有效，晚填一个月就多花 15%。

按需求对号入座：只要一台能跑活的机器，Hybrid 4GB 折后 $33.15/月最省；要 IPMI 和整机的掌控感，Entry Xeon 折后 $118/月是全系最划算的裸金属；追求单核性能就直接去犹他州找 Ryzen。👉 [确认配置，开通你的 RackNerd 独立服务器](https://bit.ly/RacKnerd)
