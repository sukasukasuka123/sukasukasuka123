# Hi ！ here is sukasukasuka123 ✋🤓

**Go 后端 / 系统方向开发者**
专注 **高并发资源管理、分布式通信机制与系统抽象设计**

> Interested in how systems behave under pressure, not just how they work in demos.

---

## 🧠 技术画像 | Technical Profile

* **主力语言**：Go
* **核心能力**：

  * 高并发编程（Goroutine / Channel / CAS）
  * 资源池与连接池抽象设计
  * 分布式系统通信模型（Gossip）
  * 系统可扩展性与失败场景分析
* **关注重点**：
  系统在 *高负载、资源竞争、不可靠网络* 下的行为

---

## 🚀 核心项目 | Selected Projects

### **TemplatePoolByGO**

> **通用弹性资源池实现（生产级设计取向）**

* 技术栈：Go
* 核心问题：
  **如何在高并发场景下安全、可控地管理有限资源**
* 关键设计：

  * 动态扩容 / 缩容（基于压力与使用率）
  * 超时等待与限流，避免雪崩
  * 资源生命周期建模（Create / Update / Expire）
  * 基于 CAS + Channel 的非阻塞调度
* 适用场景：
  数据库连接池、RPC 客户端池、外部服务资源池

🔗 [https://github.com/sukasukasuka123/TemplatePoolByGO](https://github.com/sukasukasuka123/TemplatePoolByGO)

---

### **Gossip**

> **Go 实现的分布式 Gossip 协议（偏系统实验）**

* 技术栈：Go
* 关注点：

  * 节点发现与状态传播
  * Fanout 控制与传播效率
  * 网络不稳定情况下的信息一致性
* 设计目标：
  探索 **去中心化通信模型** 在真实约束下的行为特征

🔗 [https://github.com/sukasukasuka123/Gossip](https://github.com/sukasukasuka123/Gossip)

---

### **YuanXinAvatarMan**

> **RAG 驱动的 AI 应用 Demo（工程整合方向）**

* 技术栈：JavaScript / Python
* 内容：

  * RAG 流程整合
  * 向量检索 + 生成模型协同
* 定位：
  偏 **系统整合与工程实践**，非模型训练本身

🔗 [https://github.com/sukasukasuka123/YuanXinAvatarMan](https://github.com/sukasukasuka123/YuanXinAvatarMan)

---

## 🧩 系统设计取向 | How I Think About Systems

* 倾向 **先建抽象，再谈实现**
* 关注：

  * 资源是如何被争用的
  * 压力是如何扩散的
  * 错误是如何被放大的
* 对“看起来能跑”的系统保持警惕
  更关心它在第 10 万次请求时会发生什么

---

## ✍️ 思考与记录 | Notes & Essays

* 技术设计随笔
* 系统抽象与人类行为的类比
* 对工程妥协、复杂性与边界条件的反思

🔗 [https://github.com/sukasukasuka123/-](https://github.com/sukasukasuka123/-)

---

## 📫 Contact

* GitHub: [https://github.com/sukasukasuka123](https://github.com/sukasukasuka123)
* 讨论与交流：Issues / Discussions

---

> I prefer building fewer things, but understanding them deeply.
