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
- AI、Apple、地图、金融、社交与其他服务的专项规则

它不是一个追求“大而全”的公共规则库，而是一套围绕实际设备、网络环境与个人使用习惯逐步打磨的 **Personal Network Infrastructure**。

> **目标不是堆规则，而是让每一条规则都有明确用途。**

---

### 🧭 Repository Map / 仓库导航

| 分类 | 文件示例 | 用途 |
|---|---|---|
| 🍎 Apple | [`AppleCore.list`](./AppleCore.list) · [`Apple_Intelligence.list`](./Apple_Intelligence.list) | Apple 核心服务与 Apple Intelligence 分流 |
| 🤖 AI / Productivity | [`Gamma.list`](./Gamma.list) · [`Grok_Intelligence.list`](./Grok_Intelligence.list) | AI 与生产力服务专项规则 |
| 🗺️ Maps | [`Amap.conf`](./Amap.conf) | 高德地图相关 Rewrite / 广告请求处理 |
| 🌏 Region / Direct | [`China.list`](./China.list) · [`Douyin_Direct.list`](./Douyin_Direct.list) | 中国大陆及指定服务直连策略 |
| 💬 Social | [`Discord.list`](./Discord.list) · [`Kwai.list`](./Kwai.list) | 社交与内容平台规则 |
| 🏦 Finance | [`HK_Banks.list`](./HK_Banks.list) | 香港银行及金融服务相关规则 |
| 🧩 Services | [`GitHub.list`](./GitHub.list) · [`HPJY.list`](./HPJY.list) | 独立服务和自定义场景分流 |
| 🛡️ Rewrite / Blocking | [`JD.conf`](./JD.conf) · [`KuaiShou_AdBlock.conf`](./KuaiShou_AdBlock.conf) | Rewrite、广告拦截与请求控制 |
| 🌐 DNS | [`DNS.conf`](./DNS.conf) | DNS 与解析相关配置 |

> 仓库会继续演化。新增规则时，README 也应同步增加对应入口，避免规则文件逐渐变成不可维护的“文件堆”。

---

### ⚙️ Design Principles / 设计原则

**1. 精准优先于数量**  
只保留真正有用途的规则，避免无意义地扩大匹配范围。

**2. 服务隔离**  
尽量将 Apple、AI、地图、金融、社交等不同服务拆分维护，降低单一规则文件的复杂度。

**3. 可读、可查、可维护**  
文件名应尽量直接表达用途；重要规则应保留必要注释。

**4. 不把异常当功能**  
规则失效、域名变化或服务行为变化时，应重新验证，而不是依赖历史结果。

**5. 安全边界明确**  
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
- Dedicated routing for AI, Apple, maps, finance, social platforms, and other services

This is not intended to be a massive one-size-fits-all public ruleset. It is a **personal network infrastructure repository** designed around actual devices, real network conditions, and long-term maintainability.

> **The goal is not to collect more rules. The goal is to make every rule intentional.**

---

### 🧠 Philosophy

A reliable rule stack should be:

- **Explicit** — each rule should have a clear purpose.
- **Modular** — unrelated services should not be unnecessarily coupled.
- **Maintainable** — filenames, comments, and structure should remain understandable months later.
- **Verifiable** — dynamic service behavior and domain changes should be re-checked when needed.
- **Safe** — credentials and private subscription data must never be committed to a public repository.

---

### 🚦Compatibility Note

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

### Built for control. Maintained for clarity.
### 为掌控而构建，为清晰而维护。

**Acey-s- · Personal Network Infrastructure**

</div>
