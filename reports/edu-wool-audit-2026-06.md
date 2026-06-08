# edu 羊毛全景审计 — 2026-06-08

> 对象：Jianchen Cui · HPU 在线/远程 · 泰国居住 · 目标：**长期 AI token/API 额度**

---

## 一句话结论

**Azure $100/年值得申**（部署/开源推理/代理），但**几乎跑不了 Azure OpenAI**；Google 侧**没有新的泰国学生 API 钱包**，真正值钱的仍是 **Cursor（等审核）+ Anthropic Builders（Fall 2026 窗口）+ 个人 Gmail 的 Gemini 免费 API 层**；大量「学生优惠」实为**半价订阅或培训积分**，对「长期 token」帮助有限。

---

## Azure $100 能干嘛（具体场景 + 能不能跑 AI API）

### 官方条款（ms-azr-0170p）

| 项目 | 说明 |
|------|------|
| 额度 | **$100 USD**，开通后 **12 个月内**用完 |
| 续期 | 在读学生可**每年续一次**，获新的 $100（旧额度不结转） |
| 绑卡 | **不需要**信用卡 |
| 地域 | 泰国 ✅（Azure 商业覆盖 140+ 国/地区） |
| 限制 | **每人仅 1 个** Azure for Students 订阅，不可转让、一般不可与其他优惠叠加 |
| 用完/到期 | 订阅禁用；可联系支持升级 Pay-As-You-Go 继续 |

### $100 **可以**买什么

- **计算**：B 系列 VM、Container Apps、Functions、AKS（注意配额）
- **存储/DB**：Blob、Azure SQL、Cosmos DB、PostgreSQL Flexible Server
- **AI（非 OpenAI）**：Azure AI Speech、Vision、Document Intelligence、Translator；**自托管开源模型**（Ollama/vLLM on VM）
- **网络/部署**：App Service、Static Web Apps、API Management（Developer 档）、CDN
- **附赠**：Education Hub 免费下载 VS、SQL Server Developer 等（非云积分）

### $100 **不能**买什么（官方 Exclusions）

- Azure 支持计划、Azure DevOps、Visual Studio **订阅**
- Visual Studio App Center、ExpressRoute
- **Azure Marketplace 第三方产品**
- 单独授权产品（如 Entra ID P2）

### Azure OpenAI — 能不能跑 GPT？

| 说法来源 | 结论 |
|----------|------|
| 营销页 azure.microsoft.com/free/students | 写「可访问 Azure OpenAI」 |
| Microsoft Q&A + 社区大量案例 | **Azure for Students / 免费档订阅通常无法成功部署 Azure OpenAI**，即使提交 access request |

**诚实结论**：不要把 $100 主预算押在 Azure OpenAI 上。可行路径是：

1. 大学机构订阅已开通 OpenAI（HPU 远程生大概率没有）
2. 个人 **Pay-As-You-Go** 订阅 + 单独 access approval
3. **Microsoft Founders Hub** 创业订阅

泰国 IP **不是** blocker；**订阅类型**才是。

### vs GitHub Pack 里的 Azure $100

- GitHub Student Pack **不包含独立 Azure 积分**；是引导你去 **同一套 Azure for Students** 激活
- **同一 Microsoft 账号只能有 1 份** — 不是「Pack 再送 $100」
- 你已多次 GitHub Pack 被拒 → **直接申 Azure for Students**（HPU 邮箱）更现实，不依赖 Pack

### 对本用户 AI 工作流的价值

| 场景 | 价值 | 说明 |
|------|------|------|
| 托管 API 代理 / 中间层 | ⭐⭐⭐⭐ | Container Apps + Functions，$100 够用很久 |
| 跑开源 LLM（Llama 等） | ⭐⭐⭐ | 小 VM + vLLM；$100 约能跑 1–3 月视机型 |
| Azure OpenAI GPT API | ⭐ | **不推荐作为主目标** |
| 长期每年 $100 云基础设施 | ⭐⭐⭐⭐ | 毕业前可续，适合 side project 部署 |

---

## Google 部署/工作台全景（逐项：有没有羊毛、额度、你行不行）

### 总览表

| 项目 | 学生专属？ | 额度/收益 | 泰国/HPU 远程 | 对长期 API token | 判定 |
|------|-----------|-----------|---------------|------------------|------|
| **Google AI Studio / Gemini API 免费层** | ❌ 人人有 | 低 RPM 免费（Flash ~10–15 RPM） | ✅ 个人 Gmail；❌ HPU Workspace 封 | ⭐⭐ 长期低限可用 | **立即可用** |
| **GCP $300 试用** | ❌ | $300 / 90 天，要绑卡 | ✅ | ⭐⭐⭐ 一次性 | 可选，花完即止 |
| **GCP 教务学分** | 间接 | 教授申请 → 学生领券（常 **$50/课**） | 需老师开课 | ⭐⭐⭐ 若拿到 | **被动**，远程难 |
| **Google Skills 200 积分** | ✅ | 实验课积分，**非 API 钱包**；1 年有效，可再申 | ✅ | ⭐ 学技能 | **值得申，别当 token** |
| **GEAR 计划** | ❌ | 每月 **35** Skills 积分 | ✅ | ⭐ | 顺手加 |
| **Vertex AI / Express Mode** | ❌ | 新 GCP 用户 **90 天**免账单试用（有配额） | ✅ | ⭐⭐⭐ 短期 Vertex | 新账号可试 |
| **Google AI Pro 学生 1 年** | 曾是 | Gemini App + NotebookLM Pro + 2TB | ❌ **泰国 2025-12-09 已结束**；新申 **仅美国** | — | **已死** |
| **Google AI Pro 付费 ($20/mo)** | ❌ | 含 **$10/月 GCP 积分**（需在 GDP 激活） | ✅ 可付费 | ⭐⭐⭐ $120/年云积分 | 要花钱 |
| **Google Developer Program** | 部分 | Standard 免费：35 Skills 积分/月；Premium $299/年 **2026-03-31 停售** | ✅ | ⭐⭐ | Premium 别追了 |
| **Antigravity** | ❌ | Individual **$0**，周限额 Agent | ✅ 个人 Gmail | ⭐⭐ IDE 额度 | **本周就做** |
| **Stitch** | ❌ | 免费 UI 生成（设计向） | ✅ | — | 低优先 |
| **NotebookLM** | 随 AI Pro | 免费层有限；Pro 功能需订阅 | 学生优惠已死 | ⭐ 研究笔记 | 非 API |
| **Firebase** | ❌ | Spark 免费 / Blaze 按量 | ✅ | ⭐ 托管 | 无学生加成 |
| **Cloud Run / App Engine** | ❌ | 免费层 + 上述积分抵扣 | ✅ | ⭐⭐⭐ 部署 | 配合 GCP 试用 |
| **Colab Pro 教育免费 1 年** | ✅ | 100 CU/月 | ❌ **仅美国** + 验证时人在美国 | ⭐ GPU 算力 | **你不行** |
| **Google for Startups** | ❌ | 最高 $200k（创业） | 要公司 | ⭐⭐⭐⭐ 若有项目 | 非学生路径 |
| **AI Studio vs GCP 账单** | — | **完全分离**；AI Pro/One **不包** API 用量 | — | — | 见下 |

### AI Studio vs Google Cloud 账单关系（关键）

1. **AI Studio 界面**：永久免费
2. **Gemini API 免费层**：不绑账单，低限额，数据可能用于改进模型
3. **开启 Cloud Billing** → 自动升 **Pay-as-you-go**，按 token 计费；与 Google One AI Pro **无关**
4. **GCP $300 试用积分**：主要用于 GCP 服务；Gemini API 在 AI Studio 的计费路径与纯 GCP 控制台项目可能交叉 — **启用账单前看清项目关联**
5. **Google AI Pro 的 $10/月云积分**：需在 [developers.google.com/program](https://developers.google.com/program) 手动激活并关联 billing account，可用于 Vertex AI、Cloud Run、Firebase 等

### 泰国特定 Google 项目（2026-06）

- **DE × Google 泰国 AI Pro 12 个月**：申领截止 **2025-12-09**，已结束
- **无发现** 2026 年 6 月仍开放的泰国专属 Google API 学分项目
- Colab Pro 教育、Cloudflare Students 等均 **美国限定**

---

## 仍值得薅的 .edu 清单（按长期 AI 价值排序）

| 排序 | 平台 | 收益 | 状态标签 | 说明 |
|------|------|------|----------|------|
| 1 | **Cursor 学生** | 12mo Pro ≈ $240 + 额度 | ⏳ **等 Cursor** | SheerID 人工工单进行中 |
| 2 | **Anthropic Student Builders / Fall 2026** | ~$50+ API 积分 | 🔑 **立即可盯** | Campus 春 2026 已关；education 页写 Fall 2026 开放申请 |
| 3 | **Azure for Students** | $100/年 × 在读年数 | 🔑 **立即可申** | 部署向，非 OpenAI |
| 4 | **Gemini API（个人 Gmail）** | 免费层持续 | 🔑 **立即可用** | 低限但零成本 |
| 5 | **Google Antigravity** | $0 Agent IDE | 🔑 **立即可用** | 非 token 钱包，补 Cursor 空窗 |
| 6 | **GCP $300 试用** | 90 天 $300 | 🔑 可选 | 一次性，要卡；可跑 Vertex |
| 7 | **JetBrains 学生包** | 全系 IDE 免费 | 🔑 **立即可申** | HPU 邮箱；AI Assistant 仅试用 |
| 8 | **Google Skills 200** | 培训实验 | 🔑 **立即可申** | 非 API，但零成本 |
| 9 | **Anthropic 新用户** | ~$5 | ⚠️ 低价值 | 注册赠金，一次性 |
| 10 | **Notion Education Plus** | Plus 免费 | 🔑 可试 | 非 AI token；`my.hpu.edu` 可能需 WHED 验证 |
| 11 | **Bolt.new 免费层** | ~100万 token/月 | 🔑 进行中 | 人人免费，额度有限 |
| 12 | **GitHub Pack 重试** | 含 DO $200 等 | ⏳ 材料齐后再试 | Azure 不叠加；Copilot 暂停 |
| 13 | **Perplexity Edu** | $10/mo（50% off） | ⚠️ 付费 | 研究向，非 coding API |
| 14 | **Replit / Lovable** | 50% off 订阅 | ⚠️ 付费 | 非免费 token |
| 15 | **AWS Educate** | 免费实验课 | ⚠️ 低优先 | **2026 官网已不再强调 $100 云积分**，以免费 labs 为主 |
| 16 | **Oracle Always Free** | 永久免费 VM/DB | 🔑 人人可申 | 非学生专属；$300 试用 30 天 |

---

## 明确别碰的

| 项目 | 原因 |
|------|------|
| **OpenAI Codex $100（美国/加拿大）** | 地域卡死；密歇根等为州级特例 |
| **Google AI Pro 学生 1 年（泰国）** | 2025-12-09 截止，新申仅美国 |
| **v0 Students** | HPU 不在名单 |
| **GitHub Copilot Student 新注册** | 2026/4 起暂停 |
| **Cloudflare for Students** | 仅美国 .edu + 账单邮箱 |
| **Colab Pro 教育免费** | 仅美国院校 + 验证时在美国 |
| **Kiro Students** | 仅 11 所美加大学（无 HPU） |
| **Azure OpenAI 指望 $100 学生包** | 订阅类型不支持，浪费时间 |
| **Google Skills 200 当 API 钱包** | 只能上实验课 |
| **第三方「 Claude 学生码」网站** | 无官方 Settings→Education 入口 |
| **低价值反复申 GitHub Pack** | 材料/地理未解决前纯消耗 |

---

## 推荐本周行动（最多 5 条）

1. **用 HPU 邮箱注册 Azure for Students** — 先占 $100/年订阅；规划 Container Apps / 小 VM 部署，**不碰** Azure OpenAI 申请
2. **个人 Gmail 登录 AI Studio** — 创建 API Key，记录免费层限额；Antigravity 同账号安装
3. **填 Google Skills 200 积分申请表** — 用学校邮箱，2 周内批；同时注册 GEAR 领 35/月
4. **盯 Anthropic Fall 2026 学生项目** — [anthropic.com/education](https://www.anthropic.com/education) 开放后立刻申 API credits；可先注册 console.anthropic.com 拿 $5
5. **继续推进 Cursor SheerID 人工工单** — 这是当前 **最高长期 AI 价值** 项；材料侧同步要 Summer/Fall 2026 在读证明（含 online）

---

## 来源

- [Azure for Students 条款](https://azure.microsoft.com/en-us/pricing/offers/ms-azr-0170p)
- [Azure for Students 营销页](https://azure.microsoft.com/en-us/free/students)
- [Microsoft Q&A: 学生订阅与 Azure OpenAI](https://learn.microsoft.com/en-au/answers/questions/5769429/)
- [Google Cloud for Education - Students](https://cloud.google.com/edu/students)
- [GCP 教务学分说明](https://cloud.google.com/billing/docs/how-to/edu-grants)
- [Google Skills 学生申请表](https://services.google.com/fb/forms/googlecloudskillsbooststudenttrainingcreditsapplication/)
- [Gemini 学生页 FAQ（泰国 offer 已结束）](https://gemini.google/students/)
- [Google AI Pro 学生试用帮助](https://support.google.com/gemini/answer/16417758)
- [Vertex AI Express Mode](https://cloud.google.com/vertex-ai/generative-ai/docs/start/express-mode/overview)
- [Google Developer Program](https://developers.google.com/program/plans-and-pricing)
- [Colab 高等教育公告](https://blog.google/products-and-platforms/products/education/colab-higher-education/)
- [AWS Educate](https://aws.amazon.com/education/awseducate/)
- [Kiro Students 条款](https://kiro.dev/students/terms-2026/)
- [Cloudflare for Students](https://www.cloudflare.com/students/)
- [Anthropic Education / Campus](https://www.anthropic.com/education)
