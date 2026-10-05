<a id="top"></a>

<p align="center">
  <a href="README.md">English</a> &nbsp; / &nbsp; <strong>简体中文</strong>
</p>

<a href="https://roboparty.com">
  <picture>
    <source media="(max-width: 640px)" srcset="assets/readme/hero-zh-mobile.jpg">
    <img src="assets/readme/hero-zh.jpg" alt="RoboParty RP1 全开源人形机器人。从硬件到智能，全栈开放。背景为 RP1 运动实拍。" width="100%">
  </picture>
</a>

<h1 align="center">RP1 · 全开源人形机器人</h1>

<p align="center">
  从机械、电气到固件、控制与学习，全栈开放。<br>
  让每一层都能被理解，让每一次创新都有起点。
</p>

<p align="center">
  <a href="https://roboparty.com"><strong>官网</strong></a> &nbsp; · &nbsp;
  <a href="https://roboparty.com/docs"><strong>文档</strong></a> &nbsp; · &nbsp;
  <a href="#repositories"><strong>仓库</strong></a> &nbsp; · &nbsp;
  <a href="#community"><strong>社区</strong></a>
</p>

<p align="center">
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-BeyondMimic-2950D9?style=flat-square" alt="算法：BeyondMimic" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-MiniCLite-007F86?style=flat-square" alt="算法：MiniCLite" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-UFO-27804A?style=flat-square" alt="算法：UFO" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-PBFM-4C6176?style=flat-square" alt="算法：PBFM" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-IBFM-A23D66?style=flat-square" alt="算法：IBFM" height="20"></a>
</p>

---

## 以开放为起点

**RP1 是 RoboParty 的全开源人形机器人平台：为理解、构建与拓展真实机器人，提供一个共同的研发起点。**

我们将机械与电气设计、关节模组、固件、机器人模型、部署与学习连接为完整的开发体系。你可以深入研究一个子系统，复刻一台机器人，也可以在此基础上探索自己的控制方式与学习流程。

<table width="100%">
<tr>
<td width="33%"><strong>可查阅的硬件</strong></td>
<td width="33%"><strong>可拓展的软件</strong></td>
<td width="33%"><strong>可探索的智能</strong></td>
</tr>
<tr>
<td width="33%">机械 CAD、原理图、PCB 走线、Gerber、BOM 与装配文档。</td>
<td width="33%">Linux BSP、通信、设备接口、机器人描述与部署模块。</td>
<td width="33%">行走与跑步训练、动作模仿、运动跟踪与行为模型项目。</td>
</tr>
</table>

<img src="assets/readme/rp1-gallery.jpg" alt="RP1 产品实拍，以及在摄影现场跨越高低平台的画面。" width="100%">

<p align="center"><sub>从机器人本体，到真实世界中的每一步。</sub></p>

<a id="architecture"></a>

## 一台机器人，完整的开放体系

<img src="docs/assets/architecture.svg#gh-light-mode-only" alt="RP1 控制架构：输入 / 感知 → 运控基座（运动重定向、运动策略）→ 实时控制（动作解码 · 串联解算，控制 500 Hz）→ 整机执行（ROMOMO 关节模组 · RP-hand 灵巧手），含急停与高频反馈闭环。" width="100%">
<img src="docs/assets/architecture-dark.svg#gh-dark-mode-only" alt="RP1 控制架构：输入 / 感知 → 运控基座（运动重定向、运动策略）→ 实时控制（动作解码 · 串联解算，控制 500 Hz）→ 整机执行（ROMOMO 关节模组 · RP-hand 灵巧手），含急停与高频反馈闭环。" width="100%">

**我们拒绝黑盒，没有阉割，所见即所得，把对机器人的绝对控制权完整交还开发者。**

<a id="repositories"></a>

## 仓库导航

> 具体发布内容、支持配置与安装步骤，以各子仓库维护的信息为准。

### 硬件与机器人模型

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-hardware.gif" alt="RP1 机器人本体" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_hardware"><strong>RP1_hardware</strong></a></td>
<td width="620">机械源文件、电气拓扑、原理图、PCB 走线、Gerber、线束、热管理、测试与 SOP 装配指南。</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-description.gif" alt="16 个人形机器人模型 / 3D 资源" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_description"><strong>RP1_description</strong></a></td>
<td width="620">机器人描述与几何模型：URDF、MJCF、3D 资源，以及机器人和 RPhand 配置。</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-romomo.gif" alt="ROMOMO 关节模组内部结构" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/ROMOMO"><strong>ROMOMO</strong></a></td>
<td width="620">关节模组：驱动器原理图、PCB 走线、Gerber、固件与上位机。</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-hand.gif" alt="RP Hand 灵巧手在 RP1 上的快换安装" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/rp_dexhand"><strong>rp_dexhand</strong></a></td>
<td width="620">RP Hand 灵巧手：产品与接线手册、CAN-FD 快速上手、Python/C++ SDK 接入、ROS 2 兼容说明及模型与软件资源入口。</td>
</tr>
</table>

<details>
<summary><strong>查看机器人配置与 3D 资源</strong></summary>

机器人配置与模型文件，以描述仓库当前发布版本为准。

| 配置 | 说明 |
| :--- | :--- |
| 24 DoF | 24 自由度配置 |
| 28 DoF | 固定头部配置 |
| 30 DoF | 搭载 2 自由度运动头部的配置 |
| 42 DoF | 搭载 2 自由度头部与双 RPhand 的配置 |

[机器人描述仓库](https://github.com/Roboparty/RP1_description) · [核心关节 STL](https://github.com/Roboparty/RP1_hardware/blob/main/mechanical/rp1_core_joint.stl)

</details>

### 固件与部署

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-firmware.gif" alt="RP1 计算板与 IO 端口（BSP）" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_firmware"><strong>RP1_firmware</strong></a></td>
<td width="620">Linux 底层 BSP、HPM USB-CAN、底层 SDK 与软件包源。</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-deploy.gif" alt="RP1 运行模块（电机 / 关节）" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_deploy"><strong>RP1_deploy</strong></a></td>
<td width="620">RoboParty 自研 SDK，涵盖 <code>imu</code>、<code>motor</code>、<code>dexhand</code>、<code>inference</code>、<code>camera</code> 等几大运行模块。</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-joystick.gif" alt="RP1 手柄 / 手机 App 机器人动画" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_joystick"><strong>RP1_joystick</strong></a></td>
<td width="620">RP1 手柄与手机 App 接口。</td>
</tr>
</table>

<a id="learning"></a>

### 学习与行为

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-running.gif" alt="RP1 人形机器人运行学习到的策略" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_train"><strong>RP1_train</strong></a></td>
<td width="620">行走与跑步</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-beyondmimic.gif" alt="RP1 越障行走" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_beyondmimic"><strong>RP1_beyondmimic</strong></a></td>
<td width="620">舞蹈与动作模仿</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-mimiclite.gif" alt="RP1 运动跟踪" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_mimiclite"><strong>RP1_mimiclite</strong></a></td>
<td width="620">运动跟踪</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-ufo.gif" alt="RP1 行为基础模型" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_UFO"><strong>RP1_UFO</strong></a></td>
<td width="620">行为基础模型</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-pbfm.gif" alt="RP1 感知行为基础模型" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_PBFM"><strong>RP1_PBFM</strong></a></td>
<td width="620">感知行为基础模型</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-ibfm.gif" alt="RP1 翻越障碍箱" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_IBFM"><strong>RP1_IBFM</strong></a></td>
<td width="620">交互行为基础模型</td>
</tr>
</table>

<details>
<summary><strong>相关论文</strong></summary>

- **P-BFM: Perceptive Behavioral Foundation Models for Humanoid Control via Unsupervised Reinforcement Learning** — Xue Wang, Yitang Li, Yiming Zhang, Siqin Wang, Junhan Sun, Zhihao Liu, Yaojie Shen, Jingbo Yuan, Hao Zhao, Qingdu Li. *ICLR 2027 (submission)*
- **I-BFM: Reward-Conditioned Robust Humanoid Interaction via Unsupervised Reinforcement Learning** — Ziqi Han. *ICRA (submission)*
- **MimicAll: Structured Embodiment Conditioning for Cross-Humanoid Whole-Body Motion Tracking** — Jia Li. *ICLR (submission)*
- **PREDACTOR** — action-level diffusion for on-device humanoid control — Lei Ye. *ICRA (submission)*
- **From Hitter to Player: Separating Motor Execution and Strategy in Competitive Humanoid Table Tennis** — Fanrong Dong. *ICRA (submission)*
- **Humanoid Parkour** — Fanrong Dong.
- **INTACT** — imitation-to-intent, amortized CEM, lightweight deployment — Junhan Sun. *ICLR (submission)*
- **VIStream: Bringing Inertial Sensing to Streaming Geometric Foundation Models** — Mingzhe Liu. *ICRA (submission)*

</details>

<a id="start"></a>

## 从这里开始

| 你想做什么 | 推荐入口 |
| :--- | :--- |
| **了解平台** | [开发文档与 Know-how](https://roboparty.com/docs) |
| **构建硬件** | [设计文件与装配](https://github.com/Roboparty/RP1_hardware) · [关节模组](https://github.com/Roboparty/ROMOMO) |
| **使用机器人模型** | [URDF、MJCF 与 3D 资源](https://github.com/Roboparty/RP1_description) |
| **连接与部署** | [固件与 BSP](https://github.com/Roboparty/RP1_firmware) · [运行部署](https://github.com/Roboparty/RP1_deploy) |
| **训练与探索动作** | [运动训练](https://github.com/Roboparty/RP1_train) · [动作模仿](https://github.com/Roboparty/RP1_beyondmimic) |

欢迎在对应子仓库参与贡献。本首页仓库不受理 PR；请前往相关项目提交 Issue 或 Pull Request。

<details>
<summary><strong>镜头背后</strong></summary>

<br>
<img src="assets/readme/rp1-behind-the-scenes.jpg" alt="摄影师在影棚跟拍运动中的 RP1。" width="100%">

</details>

<a id="community"></a>

## 开放共建，连接同行者

交流开发经验，分享你的项目，与 RoboParty 社区一起探索。

<p align="center">
  <a href="https://qm.qq.com/q/546376843"><img src="https://img.shields.io/badge/QQ-546376843-12B7F5?style=flat-square&logo=tencentqq&logoColor=white" alt="QQ 群：546376843" height="24"></a>
  <a href="https://t.me/roboparty"><img src="https://img.shields.io/badge/Telegram-roboparty-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram：roboparty" height="24"></a>
  <a href="https://x.com/roboparty"><img src="https://img.shields.io/badge/X-%40roboparty-181818?style=flat-square&logo=x&logoColor=white" alt="X：@roboparty" height="24"></a>
  <a href="https://roboparty.com/wechat"><img src="https://img.shields.io/badge/WeChat-roboparty-07C160?style=flat-square&logo=wechat&logoColor=white" alt="微信：roboparty" height="24"></a>
  <a href="https://discord.gg/DTcW6rR3Xa"><img src="https://img.shields.io/badge/Discord-roboparty-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord：roboparty" height="24"></a>
  <a href="https://space.bilibili.com/3546938634930456"><img src="https://img.shields.io/badge/Bilibili-roboparty-00A1D6?style=flat-square&logo=bilibili&logoColor=white" alt="哔哩哔哩：roboparty" height="24"></a>
</p>

<h3 align="center">RoboParty 生态</h3>

<p align="center">
  <a href="https://github.com/Roboparty/ROMOMO"><img src="assets/readme/romomo-card.jpg" alt="ROMOMO" width="32%"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://opengraph.githubassets.com/1/Roboparty/Party_OS" alt="Party_OS" width="32%"></a>
  <a href="https://github.com/Roboparty/roboto_origin"><img src="https://opengraph.githubassets.com/f44bef10dbc6297cb05885961f85cf827ff0fce1ddd05ab08623bc02f79d338b/Roboparty/roboto_origin" alt="roboto_origin" width="32%"></a>
</p>

---

<p align="center">
  <strong>RoboParty</strong><br>
  硬件开放，智能开放，可能性属于每一个人。
</p>

<p align="center">
  GPL-3.0 &nbsp; · &nbsp; © <a href="https://roboparty.com">RoboParty</a> &nbsp; · &nbsp; <a href="#top">返回顶部</a><br>
  <sub>各子仓库的适用许可证以其自身声明为准。</sub>
</p>
