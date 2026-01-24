# sukasukasuka123

Go 后端 / 系统方向

关注：高并发资源管理、分布式通信机制、系统可用性设计

---

## 技术栈

**语言**：Go、Python

**方向**：
- 高并发编程（Goroutine / Channel / CAS）
- 资源池与连接池设计
- 分布式通信（Gossip / 去中心化）
- 系统边界条件与失败场景处理

---

## 核心项目

### [TemplatePoolByGO](https://github.com/sukasukasuka123/TemplatePoolByGO)

**通用弹性资源池**

解决问题：高并发下安全管理有限资源，避免死锁、雪崩、资源浪费

**技术实现**：
- 泛型设计支持任意资源类型（DB / Redis / RPC 客户端）
- 快速路径无锁获取，慢路径动态创建
- Actor 模型管理状态，线程安全
- 自动重连与健康检查

**扩缩容策略**：
```
使用率 < 20%  → 快速扩容
20% ≤ 使用率 < 70% → 按比例扩容
使用率 ≥ 70% → 保守扩容
```

**架构**：
- `Pool[T]`：资源获取/归还/生命周期
- `PoolManagerActor`：扩缩容/监控
- `Conn[T]`：Create / Reset / Close / Ping 接口

---

### [Gossip](https://github.com/sukasukasuka123/Gossip)

**分布式 Gossip 协议实现**

**研究点**：
- 节点发现与状态传播
- Fanout 控制与传播效率
- 不可靠网络下的一致性保证
- 数据分块与超时重传

目标：理解去中心化通信在真实约束下的行为

---

## 工具项目

### [hardhat_helper](https://github.com/sukasukasuka123/hardhat_helper)
智能合约部署可视化工具（Python）
- 图形化部署流程
- 一键部署 + 参数可视化

### [test_helper](https://github.com/sukasukasuka123/test_helper)
面试流程管理工具（Python）
- 按类型/难度随机抽题
- 面试记录 + 数据回溯

### [xunfei_rag_uploader](https://github.com/sukasukasuka123/xunfei_rag_uploader)
讯飞 RAG 文件上传工具（Python）
- 图形化界面 + 详细日志
- 自动处理加密流程

---

## 工程方法

- 先抽象后实现
- 关注边界条件与退化路径
- 测试系统在第 10 万次请求时的行为
- 将复杂系统封装为可用工具

---

## 联系方式

GitHub: [sukasukasuka123](https://github.com/sukasukasuka123)  
Email: redred55@qq.com
