# Azure for Students

| 字段 | 值 |
|------|-----|
| 状态 | `in_progress` |
| 优先级 | P0 #2 |
| 链接 | https://azure.microsoft.com/en-us/free/students |
| 开始时间 | — |
| 完成时间 | — |

## 预期收益

- $100 Azure 积分/年（12 个月），在读可**每年续**
- 20+ 服务 12 个月免费额度 + 65+ Always Free 服务
- Education Hub 免费开发工具下载（VS、SQL Server Developer 等）
- ⚠️ **Azure OpenAI 对学生订阅基本不可用**（见下）

## 资格要求

- 18+、认证院校**全日制**学生
- 学校邮箱验证（`jcui1@my.hpu.edu`）
- **无需信用卡**
- 每人限 1 订阅；不可与多数其他优惠叠加

## 泰国/HPU 远程生适用性

- ✅ 泰国在 Azure 商业覆盖范围内
- ✅ 独立于 GitHub Pack（Pack 只是引导激活同一 offer）
- ⚠️ 条款写不接受 MOOC/营利性培训 — HPU 正式学位项目通常 OK

---

## 能干什么（实用场景）

### $100 适合花在哪

| 场景 | 推荐服务 | 对本项目价值 |
|------|----------|--------------|
| 托管 API 代理 / BFF | Container Apps、Functions、App Service | ⭐⭐⭐⭐ |
| 静态站 + 轻后端 | Static Web Apps + Functions | ⭐⭐⭐ |
| 跑开源 LLM | B 系列 VM + Docker（Ollama/vLLM） | ⭐⭐⭐ |
| 向量/RAG 实验 | Azure AI Search + Blob | ⭐⭐⭐ |
| 语音/文档 AI | Cognitive Services（非 OpenAI） | ⭐⭐ |
| 课程/实验数据库 | Azure SQL / PostgreSQL Flexible | ⭐⭐ |

### $100 不能买什么

- Azure Marketplace 第三方
- Azure DevOps、VS 订阅、支持计划、ExpressRoute
- Entra ID P2 等单独授权产品

### Azure OpenAI（GPT）— 诚实结论

- 营销页写可访问，但 **Microsoft Q&A 明确**：Azure for Students 订阅**通常无法**成功部署 Azure OpenAI，即使提交 access request
- 需要 Pay-As-You-Go / 机构订阅 / Founders Hub 等路径
- **不要把主预算押在「用 $100 跑 GPT API」上**

### 续期规则

- 12 个月到或 $100 用完 → 订阅禁用
- 仍在读 → 周年前可重新验证，获**新的** $100（旧余额不结转）
- 90 天无活动可能被回收计算资源

### vs GitHub Pack

- Pack 里的 Azure 福利 = **同一条** Azure for Students 激活链接
- **不能** Pack 再领 $100；同一 Microsoft 账号仅 1 份

---

## 申请步骤

1. 用 HPU 邮箱注册/登录 Microsoft 账号
2. 访问 https://azure.microsoft.com/en-us/free/students → Sign up
3. 学校邮箱验证学生身份
4. 在 Portal 创建订阅，记录 Subscription ID
5. **规划用途**：部署/开源推理优先，跳过 Azure OpenAI 申请

## 尝试记录

### 2026-06-08 — 第 1 次

- **操作**：访问 https://azure.microsoft.com/en-us/free/students
- **结果**：✅ 页面确认 — $100/12mo、无需信用卡、全日制大学生、学校邮箱注册、每年可续
- **卡点**：尚未点击 Sign up；需 Microsoft 账号 + 学生验证
- **下一步**：
  1. 用 HPU 邮箱创建/登录 Microsoft 账号
  2. 点 Sign up 完成学生验证
  3. 记录订阅 ID 和积分余额

### 2026-06-08 — 深度调研

- **Azure OpenAI**：社区/官方 Q&A 确认学生订阅不支持 → 更新预期收益
- **GitHub Pack**：确认不叠加，直接申本 offer 即可

## 备注

- 完整审计见 [reports/edu-wool-audit-2026-06.md](../reports/edu-wool-audit-2026-06.md)
- 条款：[ms-azr-0170p](https://azure.microsoft.com/en-us/pricing/offers/ms-azr-0170p)
