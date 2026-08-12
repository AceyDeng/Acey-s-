<div align="center">

# ⚡ Acey-s-

### Personal Network Rules & Routing Infrastructure
### 个人网络规则与分流基础设施

**A curated rule repository for cleaner routing, smarter traffic control, and a network stack built around real-world use.**  
**一个面向实际使用场景维护的个人规则仓库：更清晰的分流、更精确的流量控制，以及可长期维护的网络基础设施。**

![Status](https://img.shields.io/badge/status-active-success?style=for-the-badge)
![Rules](https://img.shields.io/badge/type-network%20rules-4c8bf5?style=for-the-badge)
![Language](https://img.shields.io/badge/docs-中文%20%2F%20English-blueviolet?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/AceyDeng/Acey-s-?style=for-the-badge)

**Built for control. Maintained for clarity.**  
**为掌控而构建，为清晰而维护。**

</div>

---

## 中文

### 这是什么？

**Acey-s-** 是一个持续维护的个人网络规则仓库，用于集中管理不同服务、应用与网络场景下的：

- 域名分流规则
- 直连 / 代理策略规则
- DNS 相关配置
- 广告与请求拦截规则
- Rewrite / MITM 配置片段
- AI、Apple、地图、金融、通信、社交、游戏与其他服务的专项规则

它不是一个追求“大而全”的公共规则库，而是一套围绕实际设备、真实网络环境与个人使用习惯逐步打磨的 **Personal Network Infrastructure**。

> **目标不是堆规则，而是让每一条规则都有明确用途。**

---

## 🌐 Featured Rule Index / 核心规则索引

这些文件属于当前长期规则栈中的核心入口。  
These files are part of the current long-term personal routing stack.

### 🤖 AI & Intelligence / AI 与智能服务

| Rule | 中文 | English |
|---|---|---|
| [`Perplexity.list`](./Perplexity.list) | Perplexity AI 核心域名规则 | Conservative Perplexity AI routing rules |
| [`Gamma.list`](./Gamma.list) | Gamma 核心服务与实时编辑相关域名 | Gamma core services and realtime editing endpoints |
| [`Grok_Intelligence.list`](./Grok_Intelligence.list) | Grok / xAI 专项域名规则 | Grok and xAI routing rules |
| [`Apple_Intelligence.list`](./Apple_Intelligence.list) | Apple Intelligence 相关服务域名 | Apple Intelligence service domains |

### 🎮 Gaming & Voice / 游戏与语音

| Rule | 中文 | English |
|---|---|---|
| [`PUBG.list`](./PUBG.list) | PUBG Mobile 相关服务域名 | PUBG Mobile related service domains |
| [`HPJY.list`](./HPJY.list) | 和平精英相关网络域名 | Routing rules for 和平精英 services |
| [`TT.list`](./TT.list) | TT 语音及相关服务域名 | TT voice and related service domains |

### 💳 Finance & Payments / 金融与支付

| Rule | 中文 | English |
|---|---|---|
| [`HK_Banks.list`](./HK_Banks.list) | 香港主要银行及相关金融服务 | Major Hong Kong banking service domains |
| [`octopus-hk.list`](./octopus-hk.list) | 香港八达通 / O! ePay 相关服务 | Hong Kong Octopus / O! ePay domains |
| [`yahoo.list`](./yahoo.list) | Yahoo Mail、Finance、News 等服务 | Yahoo Mail, Finance, News and related services |

### 📡 Telecom & Connectivity / 通信与连接

| Rule | 中文 | English |
|---|---|---|
| [`ctm-clubsim.list`](./ctm-clubsim.list) | CTM、ClubSIM、Moldtelecom、Vodafone DE、eSIM.gg 等统一策略域名 | Shared routing set for CTM, ClubSIM, Moldtelecom, Vodafone DE, eSIM.gg and related services |
| [`Tello.list`](./Tello.list) | Tello 与相关移动服务 API 域名 | Tello and related mobile-service API domains |

> 新增长期使用的规则文件时，应同步把入口加入 README。  
> When a new rule becomes part of the long-term stack, add its entry to this README as well.

---

### 🧭 Repository Map / 仓库导航

| 分类 | 文件示例 | 用途 |
|---|---|---|
| 🍎 Apple | [`AppleCore.list`](./AppleCore.list) · [`Apple_Intelligence.list`](./Apple_Intelligence.list) | Apple 核心服务与 Apple Intelligence 分流 |
| 🤖 AI / Productivity | [`Perplexity.list`](./Perplexity.list) · [`Gamma.list`](./Gamma.list) · [`Grok_Intelligence.list`](./Grok_Intelligence.list) | AI 与生产力服务专项规则 |
| 🗺️ Maps | [`Amap.conf`](./Amap.conf) | 高德地图相关 Rewrite / 广告请求处理 |
| 🌏 Region / Direct | [`China.list`](./China.list) · [`Douyin_Direct.list`](./Douyin_Direct.list) | 中国大陆及指定服务直连策略 |
| 💬 Social / Services | [`Discord.list`](./Discord.list) · [`Kwai.list`](./Kwai.list) · [`yahoo.list`](./yahoo.list) | 社交、内容与独立服务规则 |
| 🎮 Gaming | [`PUBG.list`](./PUBG.list) · [`HPJY.list`](./HPJY.list) · [`TT.list`](./TT.list) | 游戏及相关语音服务规则 |
| 🏦 Finance | [`HK_Banks.list`](./HK_Banks.list) · [`octopus-hk.list`](./octopus-hk.list) | 香港银行与支付服务规则 |
| 📡 Telecom | [`ctm-clubsim.list`](./ctm-clubsim.list) · [`Tello.list`](./Tello.list) | 移动运营商、eSIM 与通信服务规则 |
| 🛡️ Rewrite / Blocking | [`JD.conf`](./JD.conf) · [`KuaiShou_AdBlock.conf`](./KuaiShou_AdBlock.conf) | Rewrite、广告拦截与请求控制 |
| 🌐 DNS | [`DNS.conf`](./DNS.conf) | DNS 与解析相关配置 |

> 仓库会继续演化。README 应始终承担“总入口”的角色，避免规则文件逐渐变成不可维护的文件堆。

---

### ⚙️ Design Principles / 设计原则

**1. 精准优先于数量**  
只保留真正有用途的规则，避免无意义地扩大匹配范围。

**2. 服务隔离**  
尽量将 Apple、AI、地图、金融、通信、社交、游戏等不同服务拆分维护，降低单一规则文件的复杂度。

**3. 可读、可查、可维护**  
文件名应尽量直接表达用途；重要规则应保留必要注释。

**4. 不把异常当功能**  
规则失效、域名变化或服务行为变化时，应重新验证，而不是依赖历史结果。

**5. 最小影响范围**  
能只匹配目标服务，就不扩大到共享 CDN、云平台或无关域名。

**6. 安全边界明确**  
公开仓库中不应提交 API Key、Token、Cookie、私人订阅地址或其他凭据。

---

### 📦 使用方式

不同文件使用的语法可能对应不同的代理客户端或不同功能模块，因此在导入前请先确认：

1. 文件格式是否与你当前客户端兼容；
2. `.list`、`.conf`、Rewrite、MITM、DNS 等模块应放在正确位置；
3. 涉及 MITM 的配置需要正确安装并信任证书；
4. 应根据自己的策略组名称调整规则引用关系；
5. 更新后先小范围验证，再替换长期使用的生产配置。

**不要默认整仓文件可以直接无差别导入同一个客户端。**

---

## English

### What is Acey-s-?

**Acey-s-** is a continuously maintained personal repository for network routing rules and configuration fragments.

It brings together practical rules for:

- Domain-based routing
- DIRECT / proxy traffic decisions
- DNS-related configuration
- Request and advertisement blocking
- Rewrite / MITM workflows
- Dedicated routing for AI, Apple, maps, finance, telecom, social platforms, gaming, and other services

This is not intended to be a massive one-size-fits-all public ruleset. It is a **personal network infrastructure repository** designed around actual devices, real network conditions, and long-term maintainability.

> **The goal is not to collect more rules. The goal is to make every rule intentional.**

---

### 🧠 Philosophy

A reliable rule stack should be:

- **Explicit** — each rule should have a clear purpose.
- **Modular** — unrelated services should not be unnecessarily coupled.
- **Maintainable** — filenames, comments, and structure should remain understandable months later.
- **Verifiable** — dynamic service behavior and domain changes should be re-checked when needed.
- **Minimal in blast radius** — avoid unnecessarily broad shared-CDN or cloud-platform matches.
- **Safe** — credentials and private subscription data must never be committed to a public repository.

---

### 🚦 Compatibility Note

Files in this repository may use different syntaxes and may target different proxy-client modules.

Before importing a file:

- verify that the syntax matches your client;
- distinguish between rule lists, rewrite rules, MITM configuration, and DNS configuration;
- adapt policy-group names where necessary;
- test changes before deploying them into your primary configuration.

**Do not assume every file in this repository can be imported into the same client without modification.**

---

## 🔐 Security

This repository is public.

Never commit:

- API keys
- access tokens
- cookies or session credentials
- private subscription URLs
- personal certificates or private keys
- account-specific secrets

If a secret is ever committed, removing the file alone is not enough — the credential should also be rotated or revoked.

---

## 🛠 Maintenance

This repository is maintained as a living configuration set rather than a frozen release package.

When adding a new rule file:

1. Give it a clear and stable filename.
2. Keep its scope as narrow as practical.
3. Add comments where behavior is not self-explanatory.
4. Validate the target service before relying on the rule.
5. Add the new file to this README when it becomes part of the long-term rule stack.

---

<div align="center">

## ⚡ ACEY NETWORK RULESET

**Route with intent. Keep the network under control.**  
**让每一条流量，都去它该去的地方。**

**Acey-s- · Personal Network Infrastructure**

Maintained by **AceyDeng**

</div>
