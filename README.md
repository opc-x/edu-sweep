# edu-sweep

> 学生/教育 AI 福利扫荡日志 — 能薅的都薅一遍，成功失败全记录。

**仓库：** https://github.com/opc-x/edu-sweep

## 项目定位

系统化追踪并申请各类学生/教育权益（侧重 **AI token / API 积分 / 开发工具**），逐平台记录申请过程、卡点与结果，方便复盘和重试。

## 申请人档案

| 字段 | 值 |
|------|-----|
| 姓名 | Jianchen Cui |
| 学校 | Hawai'i Pacific University (HPU) |
| 学校邮箱 | `jcui1@my.hpu.edu` |
| 就读方式 | 在线 / 远程 (online / distance learning) |
| **现居地** | **泰国 (Thailand)** |
| GitHub | [opc-x](https://github.com/opc-x) |
| 学号 | 03213770 |
| 专业 | Artificial Intelligence |

## 目录结构

```
edu-sweep/
├── README.md           # 本文件
├── TRACKER.md          # 总览看板（状态一览）
├── profile.md          # 申请人资产与约束
├── platforms/          # 各平台详细日志（一平台一文件）
│   ├── cursor.md
│   ├── azure-students.md
│   └── ...
└── assets/             # 证明材料截图等（gitignore 敏感内容）
```

## 状态图例

| 状态 | 含义 |
|------|------|
| `pending` | 待申请 |
| `in_progress` | 进行中 |
| `blocked` | 卡住（需人工/材料） |
| `success` | 已到手 |
| `failed` | 明确失败 |
| `skipped` | 主动跳过（不值得/不符合） |

## 使用方式

1. 打开 `TRACKER.md` 看全局进度
2. 进入 `platforms/<name>.md` 看该平台完整流水
3. 每尝试一次就更新对应文件的时间戳和结果
