# 👋 Hi, I'm sukasukasuka123

**Go 后端 / 系统方向忠实的学徒**
关注 **高并发资源管理、分布式通信机制，以及复杂系统的可用性设计**

> I care not only about how systems work,
> but how they behave when things go wrong —
> and how to make them usable for humans.

---

## 🧠 技术画像 | Technical Profile

**主力语言**：Go
**技术取向**：系统工程 / 高并发 / 工具化

**核心能力**

* 高并发编程（Goroutine / Channel / CAS）
* 资源池、连接池等系统级抽象设计
* 分布式通信机制（Gossip、去中心化传播）
* 系统可扩展性、失败场景与压力行为分析

**工程习惯**

* 先建抽象，再写实现
* 对边界条件、退化路径保持警惕
* 不满足于“能跑”，更关心“长期是否稳定”

---

## 🧩 我如何看待系统 | How I Think About Systems

我关注的不是“功能是否完成”，而是：

* 资源在高并发下是如何被争用的
* 压力是如何在系统中扩散和放大的
* 错误是否会被隔离，还是连锁崩溃

比起 Demo，更关心系统在第 **10 万次请求** 时的状态。

---

## 🚀 核心项目 | Selected Projects

### **TemplatePoolByGO**

**通用弹性资源池（生产级设计取向）**

* 技术栈：Go
* 解决问题：
  如何在高并发场景下**安全、可控地管理有限资源**

**关键设计**

* 动态扩容 / 缩容（基于压力与使用率）
* 超时等待与限流，避免雪崩
* 资源生命周期建模（Create / Use / Expire）
* CAS + Channel 的非阻塞调度模型

**典型应用**

* 数据库连接池
* RPC / 外部服务客户端池

🔗 [https://github.com/sukasukasuka123/TemplatePoolByGO](https://github.com/sukasukasuka123/TemplatePoolByGO)

---

### **Gossip**

**分布式 Gossip 协议实验实现**

* 技术栈：Go
* 关注点：

  * 节点发现与状态传播
  * Fanout 控制与传播效率
  * 不可靠网络下的信息一致性
  * 数据分块与超时重传

目标不是“实现协议”，
而是理解**去中心化通信在真实约束下的行为模式**。

🔗 [https://github.com/sukasukasuka123/Gossip](https://github.com/sukasukasuka123/Gossip)

---

## 🛠️ 工具与界面 | Tools & GUI Applications

> 我习惯把复杂系统能力，封装成**可以直接使用的工具和界面**。

### **hardhat_helper**

**Hardhat 合约部署可视化工具**

* 技术栈：Python
* 特点：

  * 图形化界面，简化部署流程
  * 一键部署、参数可视化
  * 与脚手架工具深度集成

定位：
**降低系统操作门槛，让复杂流程“点得动、用得稳”**

🔗 [https://github.com/sukasukasuka123/hardhat_helper](https://github.com/sukasukasuka123/hardhat_helper)

---

### **test_helper**

**面试流程与题库管理工具**

* 技术栈：Python
* 功能：

  * 按类型与难度随机抽题
  * 面试过程完整记录
  * 数据可回溯

定位：
将原本“靠人记”的流程，
变成**可复用、可统计的系统**。

🔗 [https://github.com/sukasukasuka123/test_helper](https://github.com/sukasukasuka123/test_helper)

---

## 🧠 工程取向总结

* 能写系统
* 能扛并发
* 也能把系统**做成别人愿意用的工具**

---

## 📫 Contact

* GitHub: [https://github.com/sukasukasuka123](https://github.com/sukasukasuka123)
* Email: [redred55@qq.com](mailto:redred55@qq.com)

---
