# WorkBuddy 操作文档

> 腾讯出品的全场景 AI Agent 办公工作台 —— **用自然语言描述需求，WorkBuddy 自主规划、执行并交付文档 / 表格 / PPT 等可直接使用的成果。**
>
> 本手册汇总官方链接、下载安装、快速上手、扩展集成（专家 / 技能 / 连接器 MCP）、常见报错排障与安全说明，适合个人用户与企业团队。
>
> 文档更新：2026-10-12 ｜ 适用版本：桌面端 5.7.x

---

## 目录

- [一、官方链接速查](#一官方链接速查)
- [二、下载与安装](#二下载与安装)
- [三、快速上手](#三快速上手)
- [四、核心概念](#四核心概念)
- [五、扩展能力：专家 / 技能 / 连接器 / 资料库 / 自动化](#五扩展能力专家--技能--连接器--资料库--自动化)
- [六、集成与扩展开发（MCP / 技能）](#六集成与扩展开发mcp--技能)
- [七、常见报错与排障](#七常见报错与排障)
- [八、服务状态与可用性](#八服务状态与可用性)
- [九、数据安全与隐私](#九数据安全与隐私)
- [十、账户、积分与计费](#十账户积分与计费)
- [十一、参考链接汇总](#十一参考链接汇总)

---

## 一、官方链接速查

### 1. 核心链接

| 用途 | 链接 | 说明 |
|---|---|---|
| 🌐 **WorkBuddy 官网（网页入口 + 下载）** | <https://www.workbuddy.cn/> | 产品主页，点击「立即下载」获取桌面客户端 |
| 📘 **官方文档（完整使用手册）** | <https://www.workbuddy.cn/docs/workbuddy/Overview> | 文档站首页，含全部章节导航 |
| 🟢 **服务状态** | 见[第八节](#八服务状态与可用性) | 官方暂无独立公开状态页；提供替代查询方式 |

> ℹ️ **说明**：WorkBuddy 是**桌面客户端（AI Agent 工作台）**，不是 SaaS 网站；扩展能力通过 **专家 / 技能 / 连接器（MCP）** 实现，因此不存在传统意义上的"公网 REST API"。开发者请直接看第六节「集成与扩展开发」。

### 2. 全套官方入口

| 名称 | 链接 |
|---|---|
| 官网 | <https://www.workbuddy.cn/> |
| 文档站首页（简介） | <https://www.workbuddy.cn/docs/workbuddy/Overview> |
| 下载（官网入口） | <https://www.workbuddy.cn/> →「立即下载」 |
| 价格方案 | <https://www.workbuddy.cn/pricing/> |
| 更新日志（Changelog） | <https://www.workbuddy.cn/docs/workbuddy/Changelog> |
| 服务协议 | <https://rule.tencent.com/rule/202603180001> |
| 隐私保护声明 | <https://privacy.qq.com/document/preview/771d9a58551449e9a7e7445ebfe04966> |
| 反馈邮箱 | workbuddy@tencent.com |
| 提交工单 / 退款 | <https://console.cloud.tencent.com/workorder/category>（产品选择「腾讯云代码助手」）|

### 3. 文档站常驻章节（直达）

| 章节 | 链接 |
|---|---|
| WorkBuddy 简介 | <https://www.workbuddy.cn/docs/workbuddy/Overview> |
| 开启你的第一个任务 | <https://www.workbuddy.cn/docs/workbuddy/FirstTask> |
| 创建任务 | <https://www.workbuddy.cn/docs/workbuddy/Create-Task> |
| 任务管理 | <https://www.workbuddy.cn/docs/workbuddy/Task-Management> |
| 任务对话 | <https://www.workbuddy.cn/docs/workbuddy/Conversation> |
| 结果查看 | <https://www.workbuddy.cn/docs/workbuddy/Results> |
| 模型配置 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model> |
| Windows 安装指南 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Installation-Win-Guide> |
| macOS 安装指南 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Installation-Mac-Guide> |
| **常见问题 FAQ** | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/FAQ> |
| 更新日志 | <https://www.workbuddy.cn/docs/workbuddy/Changelog> |
| WorkBuddy 小程序 | <https://www.workbuddy.cn/docs/workbuddymini/quick-start/Overview> |

---

## 二、下载与安装

### 环境要求

| 平台 | 要求 |
|---|---|
| **Windows** | Windows 10 及以上，支持 x64（ARM64 支持情况以当前版本说明为准）；**不支持 Windows 7 / 8 / 8.1** |
| **macOS** | macOS 12（Monterey）及以上 |

> 不满足上述要求的系统将无法启动 WorkBuddy。

### 下载地址

1. 打开官网 **<https://www.workbuddy.cn/>**
2. 点击「**立即下载**」，按系统选择对应安装包
3. macOS 需区分芯片：**M 系列芯片选 `Mac ARM64`**，**Intel 芯片选 `Mac X64`**（无法判断时官网默认提供兼容性更好的 X64 包）

> ⚠️ 请务必从**官方渠道**下载，避免使用第三方来源的安装包。

### 安装

**Windows**

1. 双击下载的安装包，启动安装程序
2. 勾选「我同意此协议」→ 下一步
3. 选择安装路径（默认路径可直接下一步）→ 下一步
4. 确认开始菜单文件夹 → 下一步
5. 建议勾选「创建桌面快捷方式」→ 下一步
6. 确认配置无误 → 点击「安装」→ 完成后点击「完成」

**macOS**

1. 双击下载的 `.dmg` 文件，打开安装窗口
2. 将 **WorkBuddy** 图标拖入 **Applications** 文件夹
3. 等待拷贝完成，退出已挂载的磁盘映像
4. 若首次启动提示「无法验证开发者」，前往 **系统设置 → 隐私与安全性 → 安全性**，点击「仍要打开」

### 登录

1. 启动 WorkBuddy，点击「登录」，浏览器自动打开登录页（workbuddy.cn）
2. 勾选《用户服务协议》与《隐私政策》
3. 支持 **微信扫码**（推荐）、**手机号**、**邮箱**、**SSO** 等登录方式，全程在登录页完成，无需跳转
4. 页面提示登录成功后，返回客户端即可使用

### 版本更新

点击左下角**头像 → 检查更新**，系统自动检测并升级。

---

## 三、快速上手

### 认识工作界面

| 区域 | 功能 |
|---|---|
| **工具栏** | 屏幕顶部，提供「关于 WorkBuddy / 编辑 / 窗口」等常用操作 |
| **侧边栏** | 任务列表（按文件夹分组），支持搜索与管理；底部显示用户头像 |
| **对话区** | 核心交互区：任务标题栏 + 消息列表 + 输入框 |
| **结果区** | 右侧面板，「概览」与「产物」两类内容可切换查看 |

### 你的第一个任务

1. 在输入框用**自然语言**描述需求（无需拆解步骤）
2. 选择工作模式、补充必要的上下文（可用 `@文件名` 引用本地文件）
3. 提交后 WorkBuddy 自动规划并执行
4. 任务完成后，在**右侧结果区**查看产物并验收

> 建议阅读顺序：创建任务 → 任务管理 → 任务对话 → 结果查看（见[第一节 3](#3-文档站常驻章节直达)）。

### 任务状态

任务在侧边栏中会有不同状态（如进行中 / 已完成 / 失败 / 待处理 / 规划中 / 已归档），据此决定处理动作：

- **进行中** → 观察，必要时可中断调整
- **已完成** → 及时**验收并归档**，避免堆积
- **失败** → 查看报错，补齐信息后重跑
- **待处理** → 它在等你回复，最容易被遗忘
- **已归档** → 从主列表隐藏，可在数据管理中恢复或删除（归档 ≠ 删除）

---

## 四、核心概念

| 概念 | 说明 |
|---|---|
| **任务（Task）** | 一次由自然语言驱动的自主执行过程，可包含多个步骤与子代理 |
| **工作模式** | 不同执行策略（如自动执行 / 计划先审 / 只读问答等），按任务风险选择 |
| **产物（Artifacts）** | 任务交付的文档、表格、PPT、网页等文件，在结果区查看 |
| **多任务并行** | 支持同时创建并处理多个任务 |
| **本地文件操作** | 授权后可批量整理、修改本地文件 |
| **`@` 文件引用** | 用 `@文件名` 直接引用本地文件，自动读入作为上下文 |
| **斜杠命令** | 输入框中以 `/` 开头的快捷命令（如 `/model` 切换模型、`/skills` 查看技能、`/clear` 清空对话、`/help` 帮助、`/config` 设置等），实际可用命令以客户端为准 |
| **跨会话记忆** | 记住你的偏好与项目上下文，减少重复说明 |

---

## 五、扩展能力：专家 / 技能 / 连接器 / 资料库 / 自动化

WorkBuddy 通过四类可扩展能力对接不同场景：

| 能力 | 作用 | 入口 |
|---|---|---|
| **专家（Experts）** | 特定领域的角色与工作方法（如金融、法律、数据分析），相当于"换一个更专业的脑子" | 左侧边栏「专家」 |
| **技能（Skills）** | 封装专业领域知识与工作流模板，按需自动加载 | 左侧边栏「技能」/ `/skills` |
| **连接器（Connectors）** | 通过 **MCP 协议**接入外部服务与数据（如飞书、腾讯文档、GitHub、Notion 等） | 左侧边栏「连接器」 |
| **资料库（Library）** | 集中管理资料（文档 / 表格 / 网页 / 云盘文件），供任务检索、分析与生成 | 左侧边栏「资料库」 |

此外支持**自动化**能力：按计划（定时/周期）自动执行任务，适合例行化的报表汇总、信息采集与推送。

> 官方预置连接器清单（含数据存储与合规信息）：<https://www.workbuddy.cn/document/default-mcp-connectors>

---

## 六、集成与扩展开发（MCP / 技能）

> 本节即"开发者 / API 指引"。WorkBuddy 通过 **MCP（Model Context Protocol）** 协议与外部系统集成，而非传统 REST API。

### 6.1 连接器（MCP）使用文档

- 官方文档：<https://www.workbuddy.cn/docs/cli/mcp>

**传输类型**

| 类型 | 说明 |
|---|---|
| **STDIO** | 通过标准输入输出与本地进程通信（本地 MCP Server） |
| **SSE** | 通过 Server-Sent Events 与远程服务通信 |
| **HTTP** | 通过 HTTP 流式传输与远程服务通信 |

**配置作用域与优先级**

- `user`：全局用户配置，应用于所有项目
- `project`：项目级配置，应用于特定项目
- `local`：本地配置，仅当前会话/工作区

> 同名服务的生效优先级：**local > project > user**

**安全审批**：项目作用域的 MCP 服务器**首次连接需用户审批**，系统展示服务器详情后可选择批准或拒绝。

### 6.2 配置文件位置

用户级配置文件：

```
~/.workbuddy/mcp.json
```

> 该文件保存所有已安装 MCP 连接器的配置信息（command / args / env / headers 等）。

**本地（stdio）示例**

```json
{
  "mcpServers": {
    "my-local-tools": {
      "command": "node",
      "args": ["./my-mcp-server.js"],
      "env": {
        "API_TOKEN": "your-token-here"
      }
    }
  }
}
```

**远程（HTTP）示例**

```json
{
  "mcpServers": {
    "remote-service": {
      "url": "https://api.example.com/mcp/",
      "headers": {
        "x-api-key": "your-api-key-here"
      }
    }
  }
}
```

### 6.3 安装与启用连接器的通用流程

1. 打开左侧「**连接器**」管理页
2. 浏览或搜索所需的连接器 / MCP 服务
3. 点击「安装」
4. 按提示完成认证（OAuth / API Key / 账号密码）
5. 点击「**信任**」激活（**未信任不可调用**）
6. 在对话或 Agent 中使用

> 命令行添加自定义 MCP 通常还需在设置中的「自定义 MCP」入口粘贴配置并保存，然后点击「信任」启用。

### 6.4 自定义连接器

WorkBuddy 支持接入任何实现了 MCP 协议的服务（企业内部 API、第三方 SaaS、自建工具）。

> ⚠️ **责任划分**：官方预置连接器由腾讯云选择、集成与维护；**你自行添加的第三方 / 自建 MCP 服务不在默认清单内**，官方不对其身份、安全性、存储位置、跨境传输与合法性作任何承诺或背书，安全与合规责任由接入方自行承担。

### 6.5 技能（Skills）开发

- 官方文档：<https://www.workbuddy.cn/docs/cli/skills>

**核心概念**

- **Skill**：封装领域知识 / 工作流模板，由 AI **自动识别并调用**（对用户透明）
- **Slash Command**：用户手动输入的快捷命令

**目录结构**：每个技能一个独立目录，内含 `SKILL.md`

```
<项目>/.workbuddy/skills/          # 项目级技能
~/.workbuddy/skills/               # 用户级技能
├── pdf/
│   └── SKILL.md
├── data-analysis/
│   └── SKILL.md
└── code-review/
    └── SKILL.md
```

> 项目级技能可在团队成员间共享；安装第三方技能前建议先做安全审计。

---

## 七、常见报错与排障

> 完整清单请查阅官方 **<https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/FAQ>**。以下为高频问题速查。

### 7.1 一键自检：诊断工具（先做这一步）

WorkBuddy 内置「**诊断工具**」，可一键检测网络、系统资源、安全软件、环境信息与崩溃日志，并自动生成报告：

1. 顶部「**帮助 → 诊断工具**」→ 弹出诊断窗口
2. 点击「**开始检测**」，实时显示进度与结果（检测期间关闭弹窗不影响）
3. 完成后自动生成 `.txt` 报告，存于日志目录 `logs/self-check/`（保留最近 10 份）
4. 可点击「**导出报告**」或「**定位文件**」，提交反馈时一并提供

**检查项**

| 大类 | 内容 |
|---|---|
| 网络 | API 连通性、DNS、TCP 端口、代理检测、丢包率 |
| 系统资源 | 磁盘剩余空间（<1GB 报失败、<3GB 告警）、内存使用 |
| 安全软件 | EDR / 杀毒软件识别、文件读写监控检测 |
| 环境信息 | 系统信息、客户端版本、安装日志 |
| 崩溃日志 | 崩溃历史摘要 |

> 报告已脱敏（IP 仅保留前两段、用户名替换为 `***`），可安全提供给支持团队。

### 7.2 高频问题速查

| 现象 | 常见原因 | 处理 |
|---|---|---|
| **点击无反应 / 无法登录** | 未设置默认浏览器；目录权限不足；安全软件拦截 | ① 将 Chrome 设为默认浏览器，或在登录页「复制链接」后手动粘贴打开；② 检查 `%APPDATA%\CodeBuddyExtension` 目录 owner 是否为当前用户，必要时 `takeown`/`icacls` 授权（Mac 用 `chown`）；③ 临时退出**火绒 / 360 / 电脑管家 / Windows 安全中心**后重试 |
| **升级或重启后工作空间文件夹消失** | Windows 下工作空间被移动 | 到 `C:\Users\<用户名>\workbuddy`（Mac：`/Users/<用户名>/WorkBuddy`）中找到以日期或自定义名命名的文件夹，用 WorkBuddy 打开即可找回；重要文件建议另存独立目录 |
| **更新提示「安装目录下存在用户项目目录」** | 更新会清空并重写安装目录 | 打开安装目录（`C:\Users\<用户名>\AppData\Local\Programs\WorkBuddy` / `/Applications/WorkBuddy.app`），**移除对话产生的文件夹与个人文件**，仅保留 `bin`、`locales`、`resources`、`tools` 系统文件夹，再重新检查更新 |
| **整理桌面后文件疑似丢失** | 批量移动脚本执行 | 执行前**先备份**；执行后优先检查目标整理目录与**回收站** |
| **Bot 已接入但发消息无响应**（QQ / 企业微信 / 微信 / 飞书 / 钉钉） | 连接掉线 / 模型异常 | 确认连接在线 → **优先切换模型**后重测；微信场景长时间无响应可断开重连；记录复现时间与平台类型 |
| **云端部署 / 服务器安装失败** | 服务端能力仍在完善 | Windows Server / SSH 场景暂不支持，正式支持以官方后续版本为准 |

### 7.3 日志位置

| 平台 | 操作 |
|---|---|
| **Windows** | 左上角「**帮助 → 打开日志目录**」，其中的压缩包即日志 |
| **macOS** | 顶部「**帮助 → 打开日志文件夹**」，找到对应 `.zip` 日志包 |

### 7.4 反馈渠道

1. 客户端右上角「**帮助 → helpFeedback**」，或**头像 → 设置 → 帮助与反馈 → 意见反馈**
2. 描述问题 + 上传截图 + 勾选「**上传日志**」后提交
3. 或发送邮件至 **workbuddy@tencent.com**

> 日志仅用于排查问题，可能包含对话记录、设备信息等，详见隐私保护声明。

### 7.5 排障通用原则

- **优先保留证据**：错误码、报错截图、系统版本、网络环境、发生时间
- **优先最小化验证**：先切换模型 / 重连平台 / 拆分任务，再做深入定位
- **重要文件先备份**：尤其是桌面整理、批量移动、工作空间迁移等操作

---

## 八、服务状态与可用性

> **说明**：截至本文更新，WorkBuddy **暂未提供独立可公开访问的服务状态页**（网络上流传的部分状态页地址当前无法访问，请以官方渠道为准）。如需判断"是本地问题还是服务端问题"，可通过以下方式：

### 8.1 客户端自检（首选）

使用内置「**诊断工具**」（帮助 → 诊断工具），直接检测 **API 连通性 / DNS / TCP 端口 / 代理 / 丢包率**，几分钟内即可判断是否为本地网络问题。

### 8.2 腾讯云健康看板

WorkBuddy 依托腾讯云运行，可参考腾讯云官方健康看板，了解底层云服务可用性：

👉 **<https://status.cloud.tencent.com/>**

### 8.3 官方更新与公告

- 更新日志（版本迭代与修复记录）：<https://www.workbuddy.cn/docs/workbuddy/Changelog>
- 官方文档的「常见问题」页会汇总当期已知问题与处理建议

### 8.4 故障时的处理顺序

```
使用异常
 ├─ 先跑「诊断工具」→ 网络/资源/安全软件问题就地解决
 ├─ 再看更新日志 / 官方渠道 → 是否为已知的服务端问题
 ├─ 服务端问题 → 等待官方修复（本地折腾无效），可关注是否发放补偿积分
 └─ 仅自己异常 → 检查本地网络、DNS、代理、账号登录态
```

---

## 九、数据安全与隐私

WorkBuddy 采用**三层纵深防御安全架构**：

**① 技术防御层 —— 沙箱隔离与权限控制**

- **Bash 命令沙箱**：AI 操作与真实系统严格隔离
- **文件系统隔离**：仅能访问预先授权的工作空间目录
- **防沙箱逃逸**：阻止对配置文件的写入，防止恶意脚本植入
- **默认安全设计**：启动时仅拥有只读权限，编辑文件 / 运行命令需**显式用户批准**
- **分层权限系统**：`allow`（允许）/ `ask`（询问）/ `deny`（拒绝）

**② 管理管控层 —— 企业级统一管控**

- **SSO 单点登录**：统一身份认证，组织架构自动同步
- **Credit 额度控制**：按部门 / 角色差异化设置 AI 使用额度
- **IP 白名单**：限制特定 IP 段设备登录
- **精细化工具调用权限**：严格控制 AI 对文件、命令、网络的访问

**③ 合规审计层 —— 数据保护与合规**

- **Skill 安全审计**：与安全团队联动，分级风险判别
- **skill-scanner 本地安全检查**：安装前主动防御潜在风险
- **数据本地执行不上传**：数据在本地环境处理
- **服务端仅处理数据片段**：用后即弃，不保存、不用于模型训练
- 完善的用户协议与隐私协议，符合网络安全法 / 数据安全法 / 个人信息保护法

> **企业级**：提供 **VPC 专享版**（后台服务、数据库、向量数据库部署于独立 VPC，物理隔离 + 内网通信 + 数据主权）。
> 另可参考官方隐私保护声明：<https://privacy.qq.com/document/preview/771d9a58551449e9a7e7445ebfe04966>

### 使用安全建议

- ✅ 从**官方渠道**下载安装包
- ✅ 安装第三方**技能 / 连接器前先做安全审计**，不信任来源不明的 MCP 服务
- ✅ 定期检查连接器授权，及时撤销不再使用的服务
- ✅ 处理敏感数据时，确认工作空间权限与沙箱策略
- ❌ 不要在对话中提交他人隐私或涉密数据

---

## 十、账户、积分与计费

| 事项 | 说明 |
|---|---|
| **计费方式** | 按 **Credits（积分）** 消耗，不同模型消耗不同；自动化定时任务同样消耗积分 |
| **积分配额** | 新用户通常有赠送额度；企业版可按部门/角色配置额度 |
| **查询用量** | 登录官网 → 右上角头像 → 个人中心 → **套餐与用量**，查看积分余额与明细 |
| **价格方案** | <https://www.workbuddy.cn/pricing/> |
| **积分异常** | 截图发送至 workbuddy@tencent.com 核实 |
| **退款** | 登录腾讯云 → 提交工单（产品选「腾讯云代码助手」），工单 2 个工作日内审核 |
| **企业售前 / 商务** | 见价格方案页的企业版渠道 |

**省积分建议**：合理设置自动化任务频率；简单任务选用更经济的模型；避免让复杂的批量任务长时间空跑。

---

## 十一、参考链接汇总

| 名称 | 链接 |
|---|---|
| WorkBuddy 官网 | <https://www.workbuddy.cn/> |
| 文档站首页 | <https://www.workbuddy.cn/docs/workbuddy/Overview> |
| 开启第一个任务 | <https://www.workbuddy.cn/docs/workbuddy/FirstTask> |
| 创建任务 | <https://www.workbuddy.cn/docs/workbuddy/Create-Task> |
| 任务管理 | <https://www.workbuddy.cn/docs/workbuddy/Task-Management> |
| 任务对话 | <https://www.workbuddy.cn/docs/workbuddy/Conversation> |
| 结果查看 | <https://www.workbuddy.cn/docs/workbuddy/Results> |
| 模型配置 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model> |
| Windows 安装指南 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Installation-Win-Guide> |
| macOS 安装指南 | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Installation-Mac-Guide> |
| **常见问题 FAQ** | <https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/FAQ> |
| 更新日志 | <https://www.workbuddy.cn/docs/workbuddy/Changelog> |
| **MCP 使用文档** | <https://www.workbuddy.cn/docs/cli/mcp> |
| **技能系统文档** | <https://www.workbuddy.cn/docs/cli/skills> |
| 默认 MCP 连接器清单 | <https://www.workbuddy.cn/document/default-mcp-connectors> |
| WorkBuddy 小程序 | <https://www.workbuddy.cn/docs/workbuddymini/quick-start/Overview> |
| 价格方案 | <https://www.workbuddy.cn/pricing/> |
| 腾讯云健康看板（状态参考） | <https://status.cloud.tencent.com/> |
| 提交工单 / 退款 | <https://console.cloud.tencent.com/workorder/category> |
| 服务协议 | <https://rule.tencent.com/rule/202603180001> |
| 隐私保护声明 | <https://privacy.qq.com/document/preview/771d9a58551449e9a7e7445ebfe04966> |

---

## 免责声明

- 本文档为使用经验整理，**非腾讯官方文档**；产品功能、界面、链接与计费规则均可能随版本更新而变化，**请以官方文档与客户端实际表现为准**。
- 文中第三方来源整理的内容（如部分快捷命令、任务状态名称）仅供快速参考，请以客户端实际为准。
- 请遵守 WorkBuddy 服务协议、隐私政策及相关法律法规。

---

> 如果本文档对你有帮助，欢迎 Star 支持 ⭐
