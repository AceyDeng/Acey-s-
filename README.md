<div align="center">

# 🚀 Acey Shadowrocket Rules

### 精准分流 · 模块化维护 · 为真实网络环境而构建
### Precision Routing · Modular Rules · Built for Real-World Networks

**A personal Shadowrocket routing ruleset maintained by Acey.**  
**Acey 的个人 Shadowrocket 分流规则库。**

![Shadowrocket](https://img.shields.io/badge/Shadowrocket-Routing-111111?style=for-the-badge&logo=rocket&logoColor=white)
![Rules](https://img.shields.io/badge/Rules-12-2563EB?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-16A34A?style=for-the-badge)
![Language](https://img.shields.io/badge/中文-English-7C3AED?style=for-the-badge)
![Last Commit](https://img.shields.io/github/last-commit/AceyDeng/Acey-s-?style=for-the-badge)

**Route with intent. Keep the stack clean.**  
**每一条流量，都应该去它该去的地方。**

</div>

---

## 🇨🇳 中文

### 这是什么？

**Acey Shadowrocket Rules** 是一个面向个人长期使用维护的 **Shadowrocket 分流规则仓库**。

这里不追求“大而全”，也不把几万条规则简单堆在一起。仓库只保留我实际使用、值得单独维护的服务规则，让不同应用、AI 服务、游戏、金融与通信业务可以拥有更清晰、更独立的路由策略。

核心目标只有几个：

- **精准**：尽量让规则只命中真正需要处理的流量；
- **模块化**：不同服务拆分维护，减少互相污染；
- **可读**：文件名直接表达用途，方便长期维护；
- **可控**：重要服务可以独立选择节点、直连或其他策略；
- **克制**：不为了“规则多”而增加没有明确用途的条目。

> **这不是一个规则垃圾场，而是一套属于自己的 Shadowrocket 路由层。**

---

## 🧭 Rule Directory / 规则导航

| 分类 | 规则文件 | 主要用途 |
|---|---|---|
| 🤖 AI | [`Perplexity.list`](./Perplexity.list) | Perplexity 相关流量 |
| 🤖 AI / Productivity | [`Gamma.list`](./Gamma.list) | Gamma 相关流量 |
| 🤖 AI | [`Grok_Intelligence.list`](./Grok_Intelligence.list) | Grok / xAI Intelligence 相关流量 |
| 🍎 Apple AI | [`Apple_Intelligence.list`](./Apple_Intelligence.list) | Apple Intelligence 相关流量 |
| 🎮 Gaming | [`PUBG.list`](./PUBG.list) | PUBG 相关流量 |
| 🎮 Gaming | [`HPJY.list`](./HPJY.list) | 和平精英相关流量 |
| 🏦 Finance | [`HK_Banks.list`](./HK_Banks.list) | 香港银行及金融服务 |
| 💳 Payment | [`octopus-hk.list`](./octopus-hk.list) | 香港八达通相关服务 |
| 📶 Telecom | [`ctm-clubsim.list`](./ctm-clubsim.list) | CTM / Club SIM 相关服务 |
| 📶 Telecom | [`Tello.list`](./Tello.list) | Tello 相关服务 |
| 🎵 Social / Media | [`TT.list`](./TT.list) | TT / TikTok 相关流量 |
| 🌐 Web Services | [`yahoo.list`](./yahoo.list) | Yahoo 相关流量 |

---

## ⚙️ 设计理念

### 01 — Service Isolation / 服务隔离

AI、游戏、金融、通信等服务尽可能拆成独立规则文件。一个服务发生域名变化时，不需要动整套配置。

### 02 — Explicit Routing / 明确路由

规则存在的目的，是让某类流量进入明确的策略，而不是依赖模糊、不可解释的大范围匹配。

### 03 — Small but Intentional / 少而明确

这个仓库不以规则数量为目标。**能用 20 条解决的问题，不需要用 2,000 条证明它很复杂。**

### 04 — Maintainability First / 可维护性优先

任何长期规则都应该做到：过几个月重新打开时，依然能看懂它为什么存在、服务于什么场景。

### 05 — Real-World Validation / 真实环境验证

服务域名、CDN、API 与客户端行为都会变化。历史可用不等于永久有效；重要规则应在实际网络环境中持续验证。

---

## 📦 使用方式

本仓库主要用于 **Shadowrocket** 的个人分流体系。

不同 `.list` 文件的具体语法和接入方式可能不同。使用前建议：

1. 打开对应规则文件并确认当前内容；
2. 根据文件语法，将其作为规则源或合并进自己的 Shadowrocket 配置；
3. 将目标规则绑定到正确的策略组；
4. 更新后先验证目标 App / 服务是否正常；
5. 不要把所有服务无差别绑定到同一个节点。

> **分流的价值不是“全部代理”，而是让不同流量使用最合适的路径。**

---

## 🛡️ Security / 安全

这是一个公开仓库。

**禁止提交：**

- API Key
- Access Token
- Cookie / Session
- 私人订阅链接
- 私有证书或私钥
- 任何账号级敏感凭据

如果凭据曾经被提交到 Git 历史中，仅删除文件并不等于安全，应同时撤销或轮换对应凭据。

---

## 🔧 Maintenance / 维护约定

后续新增长期使用的规则时：

1. 使用清晰、稳定的文件名；
2. 尽量保持单文件单一职责；
3. 不确定的域名不要为了“看起来完整”而硬加；
4. 服务行为改变时重新验证规则；
5. 新增长期规则后，同步更新本 README 的规则导航。

---

## 🇬🇧 English

### What is this?

**Acey Shadowrocket Rules** is a personal, continuously maintained routing rules repository built around **Shadowrocket**.

The goal is not to become a giant universal ruleset. The goal is to keep a small, intentional, modular routing layer for the services that actually matter in daily use.

The repository focuses on:

- **Precision** — match only the traffic that needs special handling;
- **Modularity** — keep unrelated services in separate rule files;
- **Clarity** — make every file easy to identify and maintain;
- **Control** — allow important services to use independent routing policies;
- **Restraint** — avoid adding rules simply to make the repository look larger.

> **This is not a rule dump. It is a personal routing layer.**

---

## 🧠 Philosophy

A good routing stack should be **explicit, modular, testable, and maintainable**.

Traffic behavior changes. Domains change. APIs move. CDN architecture evolves. A rule that worked months ago is not automatically ground truth today.

That is why this repository favors a smaller set of rules with clear intent over an oversized configuration that nobody can confidently explain.

---

## 🚦Usage Notes

These files are maintained for a Shadowrocket-based setup, but individual `.list` files may use different rule syntaxes or integration styles.

Before using a rule file:

- inspect its current syntax;
- connect it to the correct policy group;
- validate the target service after changes;
- keep unrelated services isolated where practical;
- avoid assuming that every file should use the same exit node.

**Good routing is not about proxying everything. It is about choosing the right path for each class of traffic.**

---

<div align="center">

### Built for control. Tuned for clarity.
### 为掌控而构建，为清晰而调校。

**Acey Shadowrocket Rules**  
`Precision · Control · Maintainability`

</div>
