# Google Cloud / 部署 / 工作台 全景

| 字段 | 值 |
|------|-----|
| 状态 | `reference` |
| 优先级 | P0（与 google-gemini.md、google-skills.md 联动） |
| 链接 | https://cloud.google.com/edu/students |
| 更新 | 2026-06-08 深度调研 |

> 本文件汇总 GCP、Vertex、Firebase、部署栈及 Google 开发者计划的**学生/免费**路径。API 密钥细节见 [google-gemini.md](google-gemini.md)。

---

## 快速判定（Jianchen / 泰国 / HPU）

| 路径 | 能拿 API token？ | 标签 |
|------|------------------|------|
| 个人 Gmail + AI Studio 免费层 | 低限免费，长期 | ✅ 立即可用 |
| GCP $300 试用 | 90 天，Vertex/Run 等 | ✅ 可选（要卡） |
| Google Skills 200 | ❌ 仅实验课 | ✅ 值得申 |
| 教务 GCP 学分 | 若教授发券，$50 级 | ⚠️ 被动 |
| Google AI Pro 学生 1 年 | ❌ 泰国已死 | ❌ 别碰 |
| Google AI Pro 付费 $20/mo | $10/mo 云积分 | ⚠️ 要花钱 |
| Colab Pro 教育 | ❌ 仅美国 | ❌ 你不行 |

---

## 1. Google Cloud Platform

### $300 免费试用

- **链接**：https://cloud.google.com/free
- **额度**：$300 / **90 天**
- **要求**：信用卡验证（一般不扣费除非超免费层）
- **用途**：Vertex AI、Cloud Run、Compute、BigQuery 等**几乎全部 GCP 服务**
- **学生专属**：❌ 人人一次；泰国 ✅

### 教务学分（Faculty Grants）

- **链接**：https://cloud.google.com/billing/docs/how-to/edu-grants
- 教授申请 → 学生收邮件验证 → 兑换 coupon（常见 **$50/课程**）
- 有效期兑换后 **1 年**；免费层用量**不扣**学分
- HPU 远程生：**除非某课老师申请**，否则拿不到

---

## 2. Vertex AI / Gemini on GCP

| 模式 | 说明 |
|------|------|
| **AI Studio + Gemini API** | 免费层 / 绑账单后按 token 计费；见 google-gemini.md |
| **Vertex AI Express Mode** | 新 GCP 用户 **90 天**免账单试用（有配额）；https://cloud.google.com/vertex-ai/generative-ai/docs/start/express-mode/overview |
| **Vertex AI 正式** | 需 billing；$300 试用可抵扣 |

**账单关系**：Google One / AI Pro **消费者订阅不覆盖** AI Studio API 用量。AI Pro 订阅者可通过 Google Developer Program 领 **$10/月 GCP 积分**（需手动激活到 billing account）。

---

## 3. Google AI Studio vs Google Cloud

```
AI Studio 界面 ──免费──> 原型/测试
       │
       ├─ 不绑账单 → Gemini API 免费层（低 RPM，数据可能用于训练）
       │
       └─ 绑 Cloud Billing → Pay-as-you-go（按 token，升 Tier 限额）

GCP 控制台项目 ←── 同一 Google 账号可关联，但计费逻辑分开管理
```

- HPU `my.hpu.edu`：**Workspace 封 AI Studio** → 必须用个人 Gmail（如 lijianya866@gmail.com）

---

## 4. Firebase

- **Spark**：免费，有限额
- **Blaze**：按量；无学生专属折扣
- 可用 GCP 试用/AI Pro 云积分抵扣 Blaze 用量

---

## 5. 部署：Cloud Run / App Engine

- **Cloud Run**：有永久免费层（每月一定 vCPU-秒、请求数）
- **App Engine**：免费层有限
- 配合 $300 试用或 AI Pro 的 $10/月积分部署 side project
- **泰国**：✅

---

## 6. Google Skills（培训积分）

- 学生 **200 积分** / 1 年：https://services.google.com/fb/forms/googlecloudskillsbooststudenttrainingcreditsapplication/
- **GEAR**：每月 **35** 积分 — https://www.skills.google/
- ⚠️ **不是 API 钱包**；只能上 Skills 实验和 badge

---

## 7. Colab

| 档位 | 学生福利 |
|------|----------|
| 免费 | 人人有，GPU 受限 |
| Colab Pro 教育 1 年免费 | **仅美国**院校 + SheerID + 验证时人在美国 |
| **泰国 HPU 远程**：❌ 不符合 |

---

## 8. Google Developer Program

- **Standard**：免费；GEAR 35 Skills 积分/月
- **Premium $299/年**：**2026-03-31 起停售**；权益并入 Google AI Pro/Ultra
- **AI Pro 订阅者**：$10/月 GCP 积分 + Code Assist 等 → 在 developers.google.com/program 激活
- **AI Ultra**：$100/月云积分

---

## 9. Antigravity / Stitch / NotebookLM

| 产品 | 学生路径 | 说明 |
|------|----------|------|
| **Antigravity** | ❌ 无；Individual $0 | 见 [google-antigravity.md](google-antigravity.md) |
| **Stitch** | ❌ 无 | UI 设计，见 [google-stitch.md](google-stitch.md) |
| **NotebookLM** | 随 Google AI Pro | 泰国学生 1 年优惠已结束；免费层功能有限 |

---

## 10. Google for Startups

- 最高 **$200k** 云积分 — 需创业公司，非学生专属
- 若有 side project 可注册公司后走 Activate/Startups 路径（另一赛道）

---

## 11. 泰国特定（2026-06）

- **DE × Google 泰国 AI Pro 12 个月**：截止 **2025-12-09**，已结束
- **新 Google AI Pro 学生试用**：官方帮助文档写**现仅对美国新申学生开放**；泰国曾领用户可用至原到期日
- **无**发现 2026 年 6 月仍开放的泰国专属 GCP API 学分项目

---

## 推荐动作

1. 个人 Gmail → AI Studio API Key（免费层）
2. 申 Google Skills 200 + 注册 GEAR
3. （可选）GCP $300 试用 → Vertex Express / Cloud Run 部署
4. **不要**花时间找泰国 Google AI Pro 学生续期

## 相关文件

- [google-gemini.md](google-gemini.md) — API 密钥与 Workspace 封锁
- [google-skills.md](google-skills.md) — 200 积分申请
- [gcp-trial.md](gcp-trial.md) — $300 试用
- [google-antigravity.md](google-antigravity.md)
- [reports/edu-wool-audit-2026-06.md](../reports/edu-wool-audit-2026-06.md)
