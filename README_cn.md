# Sandwich-Box
An open-source, modular edge computing and smart home hub platform. 

中文 | "English" (README_en.md)

一个重新定义边缘计算与智能家居中枢的开源硬件平台。

"Sandwich Box" 是一个开创性的模块化计算平台，其核心设计理念是 “大脑与手脚分离” 的异构架构。它通过强大的主控处理器管理全局，并驱动庞大的ESP32-S3协处理器集群来处理高并发I/O任务，为智能家居、工业自动化、边缘AI和开发者提供了一个前所未有的全能开发平台。

✨ 核心特性

🧠 强大的“大脑” (主控单元)

* 可选方案：
   * Pro/工业版: 双rk3568 SoC，提供顶级算力。
   * 家庭版: 单SoC，平衡性能与功耗。
* 运行完整的Linux系统，支持Docker容器，轻松部署复杂应用。
* 丰富的接口: 千兆以太网、多个USB端口、HDMI输出、PCIe 扩展。

🦾 无限的“手脚” (协处理单元)

* 可扩展的ESP32-S3协处理器集群，通过定制背板可连接多个ESP32模块。
* 每个ESP32-S3都是一个独立的实时处理单元，专用于传感器数据采集、设备控制、PWM输出等高并发、低延迟任务。
* 主控与协处理器之间通过高速USB或以太网通信，实现高效协同。

🧩 模块化设计

* 核心板 + 功能背板 结构，未来可升级不同性能的核心。
* 开放式扩展卡插槽，支持社区开发各种功能扩展卡（如LoRa、Zigbee、电机驱动、PoE等）。

🚀 应用场景

* 智能家居超级中枢: 同时管理全家所有设备，本地运行Home Assistant，无需云依赖。
* 工业边缘计算网关: 采集PLC、传感器数据，进行协议转换和边缘AI推理。
* 多媒体中心: 4K视频播放与游戏串流，由强大的SoC驱动。
* 开发者与极客的梦想平台: 为物联网、机器人、自动化项目提供极致的灵活性和性能。
* 教育平台: 学习Linux、嵌入式系统、网络协议和分布式计算的完美硬件。

📖 项目状态与路线图

本项目正处于早期开发阶段。我们正在积极进行硬件原理图设计和社区建设。

* Phase 1: 完成第一版原理图设计 (正在进行中)
* Phase 2: PCB布局、打样与调试
* Phase 3: 基础软件系统与固件开发
* Phase 4: 首批开发者套件测试
* Phase 5: 正式开源发布与社区推广

"查看完整的项目路线图与讨论" (https://github.com/Omerlikey/Sandwich-Box)

🤝 如何参与 & 贡献

我们坚信开源的力量，并热烈欢迎任何形式的贡献！无论您是硬件工程师、软件开发者、文档撰写者还是热情的爱好者，这里都有您的用武之地。

以下是您可以参与的方式：

1. 加入讨论: 在 "GitHub Discussions" (https://github.com/Omerlikey/Sandwich-Box/discussions) 中分享您的想法，这是我们策划一切的中心。
2. 贡献代码/设计: 查看 "开放中的Issue" (https://github.com/Omerlikey/Sandwich-Box/issues)，挑选您感兴趣的任务。
3. 完善文档: 帮助翻译、编写教程或修复文档错误。
4. 传播分享: 简单地告诉更多的人关于这个项目的存在，就是巨大的帮助！

请阅读我们的 "贡献指南" (CONTRIBUTING.md) 以了解更多细节。

🛠️ 技术概览

* 主处理器:  rk3568 x2 &a133
* 协处理器: 多颗ESP32-S3
* 内存: LPDDR4
* 存储: eMMC 
* 网络: 千兆以太网, 可选Wi-Fi 6扩展
* 视频输出: HDMI
* 扩展: PCIe , USB 3.0, GPIO, 专用背板接口
* 操作系统: Linux (基于Buildroot)

📜 许可证

本项目的硬件设计（包括原理图、PCB布局）采用 "Solderpad Hardware License v2.1" (LICENSE.md)。

本项目中的软件代码均采用宽松的 "MIT License" (LICENSE-SOFTWARE.md) 许可证。

文档采用 "Creative Commons Attribution 4.0 International License" (https://creativecommons.org/licenses/by/4.0/) 许可。

📞 联系我们 & 链接

* 项目讨论: "GitHub Discussions" (https://github.com/Omerlikey/Sandwich-Box/discussions)
* 问题反馈: "GitHub Issues" (https://github.com/Omerlikey/Sandwich-Box/issues)
* 项目创始人: Omerlikey(Omerlikey@outlook.com)

欢迎登船！让我们一起打造一些真正酷的东西。 🚀
