# Cursor 学生计划

| 字段 | 值 |
|------|-----|
| 状态 | `in_progress` |
| 优先级 | P0 #1 |
| 链接 | https://cursor.com/students |
| 开始时间 | 2026-06-08 |
| 完成时间 | — |

## 预期收益

- 12 个月 Cursor Pro 免费（≈ $240）
- 每月 $20 frontier model 用量额度
- Agent、MCP 等 Pro 功能

## 资格要求

- 在读大学生
- `.edu` 邮箱（Cursor 账号邮箱需与学校邮箱一致）
- SheerID 验证（学生证/课表/在读证明，通常 3 个月内）

## 泰国/HPU 远程生适用性

- ✅ HPU `my.hpu.edu` 符合 US `.edu`
- ✅ 居住地泰国一般不限
- ⚠️ Cursor 账号必须用 `jcui1@my.hpu.edu` 注册/登录

## 申请步骤

1. 用 `jcui1@my.hpu.edu` 登录 Cursor
2. 打开 https://cursor.com/students → Verify Status
3. SheerID 填学校信息 + 上传证明
4. 通过后 Pro 自动开通
5. **设 11 个月后取消提醒**（否则 $20/mo 自动续费）

## 尝试记录

### 2026-06-08 — 第 3 次（提交 + 邮件验证失败）

- **操作**：填 DOB `1990-01-22`，提交表单 → 收邮件 `verify@sheerid.com` → 点 Finish Verifying 链接
- **结果**：❌ **Error: We are unable to verify you at this time**
- **分析**：
  - Cursor 已用 `jcui1@my.hpu.edu` 登录 ✅
  - SheerID **邮件环验证**对 HPU `my.hpu.edu` 即时失败，**未进入文档上传步骤**
  - 尝试了 2 个 verificationId 均失败
  - 在读证明 Spring 2026 已于 5/10 结束，学生证无日期 — 即使走人工也可能被拒
- **下一步**：
  1. 联系 SheerID 人工审核：https://support.sheerid.com/en-US/help-center/contact-form
  2. 或 Cursor 论坛帖：https://forum.cursor.com/t/student-verification-issues/133734
  3. **暂停重复提交**（防 Verification Limit Exceeded）
  4. 向 HPU 要 Summer/Fall 2026 在读证明后再申

### 2026-06-08 — 第 2 次（SheerID）

- **操作**：打开 SheerID 链接，预填表单
- **已填**：
  - Country: **United States**（学校所在国，不是泰国）
  - School: **Hawaii Pacific University, Honolulu, HI**
  - Name: **Jianchen Cui**
  - Email: **jcui1@my.hpu.edu**
- **材料已备**（`assets/cursor/`，gitignore）：
  - `student-id-front.png` — Jianchen Cui, 03213770, HPU
  - `enrollment-spring2026.pdf` — Spring 2026 全日制 12 学分（⚠️ 学期 5/10 已结束，可能被要求补 Summer/Fall 证明）
- **待用户填**：Date of birth（出生月/日/年）— **唯一卡点**
- **Stripe 绑卡**：UnionBank Visa Debit 可用；**勿在聊天发 CVV**
- **卡点**：SheerID 这步**不要卡**；菲律宾 Visa 留给后面 Stripe 绑卡用
- **下一步**：填 DOB → Verify → 可能收 HPU 邮箱验证邮件或要求上传在读证明

### 2026-06-08 — 第 1 次

- **操作**：打开 https://cursor.com/students → 点 Apply → 跳转 `authenticator.cursor.sh` 登录页
- **结果**：未登录 Cursor；页面要求 Email / Google / GitHub / Apple 登录
- **卡点**：**必须用 `jcui1@my.hpu.edu` 注册/登录 Cursor**（FAQ 写明邮箱需与学校邮箱一致）；需用户本人在浏览器完成 OAuth
- **下一步**：
  1. 用 HPU 邮箱注册 Cursor（或 Google 登录选 jcui1@my.hpu.edu）
  2. 登录后 Dashboard → Settings → Students → SheerID 验证
  3. 上传 HPU 在读证明/课表（最好含 online learning 字样）

## 截图/凭证

`assets/cursor/`

## 备注

最高优先级；与 Windsurf 相比性价比最高。
