<a id="top"></a>

<p align="center">
  <strong>English</strong> &nbsp; / &nbsp; <a href="README.zh-CN.md">简体中文</a>
</p>

<a href="https://roboparty.com">
  <picture>
    <source media="(max-width: 640px)" srcset="assets/readme/hero-en-mobile.jpg">
    <img src="assets/readme/hero-en.jpg" alt="RoboParty RP1. Fully open-source humanoid platform. Open hardware. Open intelligence. RP1 photographed in motion." width="100%">
  </picture>
</a>

<h1 align="center">RP1 · Fully Open-Source Humanoid</h1>

<p align="center">
  From mechanical design and electronics to firmware, control and learning.<br>
  Built to be understood. Open to be built upon.
</p>

<p align="center">
  <a href="https://roboparty.com"><strong>Website</strong></a> &nbsp; · &nbsp;
  <a href="https://roboparty.com/docs"><strong>Documentation</strong></a> &nbsp; · &nbsp;
  <a href="#repositories"><strong>Repositories</strong></a> &nbsp; · &nbsp;
  <a href="#community"><strong>Community</strong></a>
</p>

<p align="center">
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-BeyondMimic-2950D9?style=flat-square" alt="Algorithm: BeyondMimic" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-MiniCLite-007F86?style=flat-square" alt="Algorithm: MiniCLite" height="20"></a>
  <a href="#learning"><img src="https://img.shields.io/badge/Algorithm-UFO-27804A?style=flat-square" alt="Algorithm: UFO" height="20"></a>
</p>

---

## Open by Design

**RP1 is RoboParty's fully open-source humanoid platform: a shared foundation for building, understanding and extending a real robot.**

The platform brings mechanical and electrical design, joint modules, firmware, robot models, deployment and learning into one connected development stack. Explore a single subsystem, reproduce a build, or develop your own control and learning workflows.

<table width="100%">
<tr>
<td width="33%"><strong>Hardware you can inspect</strong></td>
<td width="33%"><strong>Software you can extend</strong></td>
<td width="33%"><strong>Intelligence you can explore</strong></td>
</tr>
<tr>
<td width="33%">Mechanical CAD, schematics, PCB layouts, Gerber files, BOM and assembly documentation.</td>
<td width="33%">Linux BSP, communication, device interfaces, robot descriptions and deployment modules.</td>
<td width="33%">Locomotion training, motion imitation, tracking and behavior-model projects.</td>
</tr>
</table>

<img src="assets/readme/rp1-gallery.gif" alt="RP1 product portrait alongside an on-set photograph of RP1 stepping across raised platforms." width="100%">

<p align="center"><sub>RP1, photographed in the real world.</sub></p>

<a id="architecture"></a>

## One Robot. A Connected Stack.

<img src="docs/assets/architecture-en.svg#gh-light-mode-only" alt="RP1 control architecture: input / perception → motion control base (motion retargeting, motion policies) → real-time control (action decoding + serial-link solving at 500 Hz) → whole-body execution (ROMOMO joint modules, RP-hand), with an E-stop and a high-frequency feedback loop." width="100%">
<img src="docs/assets/architecture-en-dark.svg#gh-dark-mode-only" alt="RP1 control architecture: input / perception → motion control base (motion retargeting, motion policies) → real-time control (action decoding + serial-link solving at 500 Hz) → whole-body execution (ROMOMO joint modules, RP-hand), with an E-stop and a high-frequency feedback loop." width="100%">

**No black boxes, nothing withheld — full control handed back to the developer.**

<a id="repositories"></a>

## Explore the Repositories

> Release contents, supported configurations and setup instructions are maintained in each repository.

### Hardware & Robot Models

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-hardware.gif" alt="RP1 humanoid hardware" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_hardware"><strong>RP1_hardware</strong></a></td>
<td width="620">Mechanical source files, electrical topology, schematics, PCB layouts, Gerber files, wiring, thermal design, testing and SOP assembly guides.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-description.gif" alt="Sixteen humanoid robot models / 3D assets" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_description"><strong>RP1_description</strong></a></td>
<td width="620">Robot descriptions and geometry: URDF, MJCF and 3D assets; robot and RPhand configurations.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-romomo.gif" alt="ROMOMO joint module internals" width="200"></td>
<td width="150"><a href="https://github.com/orgs/Roboparty/teams/romomo"><strong>ROMOMO</strong></a></td>
<td width="620">Joint modules: driver schematics, PCB layouts, Gerber files, firmware and host tools.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-hand.gif" alt="RP Hand quick-swap dexterous hand on RP1" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/rp_dexhand"><strong>RP-hand</strong></a></td>
<td width="620">RP Hand: product and wiring guides, CAN-FD quick start, Python/C++ SDK integration, ROS 2 compatibility, and model and software resource links.</td>
</tr>
</table>

<details>
<summary><strong>Robot configurations & 3D asset</strong></summary>

See the description repository for model files and currently supported configurations.

| Configuration | Description |
| :--- | :--- |
| 24 DoF | 24-DoF configuration |
| 28 DoF | Fixed-head configuration |
| 30 DoF | Configuration with a 2-DoF locomotion head |
| 42 DoF | Configuration with a 2-DoF head and two RPhands |

[Robot description repository](https://github.com/Roboparty/RP1_description) · [Core joint STL](https://github.com/Roboparty/RP1_hardware/blob/main/mechanical/rp1_core_joint.stl)

</details>

### Supply Chain

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-supplychain.svg" alt="Supply-chain know-how: selection, where it is used, gates and acceptance" width="200"></td>
<td width="150"><a href="https://github.com/Taicushier-0212/rp-supplychain-knowhow"><strong>RP_supplychain</strong></a></td>
<td width="620">Humanoid supply-chain know-how: what each part is, where it is used, how to choose and inspect it, plus gates and acceptance criteria.</td>
</tr>
</table>

### Firmware & Deployment

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-firmware.gif" alt="RP1 compute board and IO ports (BSP)" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_firmware"><strong>RP1_firmware</strong></a></td>
<td width="620">Linux BSP, HPM USB-CAN bridge, low-level SDK and software package sources.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-deploy.gif" alt="RP1 runtime modules (motor / joint)" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_deploy"><strong>RP1_deploy</strong></a></td>
<td width="620">RoboParty's in-house SDK, covering runtime modules for <code>imu</code>, <code>motor</code>, <code>dexhand</code>, <code>inference</code> and <code>camera</code>.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-test.gif" alt="RP1 walking across a raised block obstacle course during full-machine testing" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/rp1_test"><strong>RP1_TEST</strong></a></td>
<td width="620">RP1 full-machine testing.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-joystick.gif" alt="RP1 joystick / mobile app robot animation" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/roboparty_joystick"><strong>roboparty_joystick</strong></a></td>
<td width="620">Controller and mobile app interfaces for RP1.</td>
</tr>
</table>

<a id="learning"></a>

### Learning & Behavior

<table width="100%">
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-running.gif" alt="RP1 humanoid running a learned policy" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/RP1_train"><strong>RP1_train</strong></a></td>
<td width="620">Walking and running, motion imitation and behavior foundation models.</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-beyondmimic.gif" alt="RP1 traversing a block obstacle course" width="200"></td>
<td width="150"><strong>RP1_beyondmimic</strong></td>
<td width="620">Dance and motion imitation</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-mimiclite.gif" alt="RP1 motion tracking" width="200"></td>
<td width="150"><strong>RP1_mimiclite</strong></td>
<td width="620">Motion tracking</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-ufo.gif" alt="RP1 behavior foundation model" width="200"></td>
<td width="150"><strong>RP1_UFO</strong></td>
<td width="620">Behavior foundation model</td>
</tr>
<tr>
<td align="center" width="200"><img src="assets/readme/rp1-data.gif" alt="Humanoid motion-capture training data: many skeletons walking" width="200"></td>
<td width="150"><a href="https://github.com/Roboparty/rp1_data"><strong>RP1_DATA</strong></a></td>
<td width="620">Training datasets.</td>
</tr>
</table>

<details>
<summary><strong>Related papers</strong></summary>

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

## Build From Here

| Your starting point | Where to go |
| :--- | :--- |
| **Understand the platform** | [Documentation & know-how](https://roboparty.com/docs) |
| **Review the supply chain** | [Component know-how & gates](https://github.com/Taicushier-0212/rp-supplychain-knowhow) |
| **Build the hardware** | [Design files & assembly](https://github.com/Roboparty/RP1_hardware) · [Joint modules](https://github.com/orgs/Roboparty/teams/romomo) |
| **Work with robot models** | [URDF, MJCF & 3D assets](https://github.com/Roboparty/RP1_description) |
| **Connect and deploy** | [Firmware & BSP](https://github.com/Roboparty/RP1_firmware) · [Deployment](https://github.com/Roboparty/RP1_deploy) |
| **Train and explore motion** | [Locomotion training](https://github.com/Roboparty/RP1_train) · [Motion imitation](https://github.com/Roboparty/RP1_train) |

Contributions belong in the relevant sub-repository. This overview repository does not accept pull requests; please open issues and pull requests in the project you are working on.

<details>
<summary><strong>Behind the scenes</strong></summary>

<br>
<img src="assets/readme/rp1-behind-the-scenes.jpg" alt="A camera operator filming RP1 in motion in the studio." width="100%">

</details>

<a id="community"></a>

## Built in the Open. Built Together.

Meet the community, share your work, and connect with RoboParty.

<p align="center">
  <a href="https://qm.qq.com/q/546376843"><img src="https://img.shields.io/badge/QQ-546376843-12B7F5?style=flat-square&logo=tencentqq&logoColor=white" alt="QQ group 546376843" height="24"></a>
  <a href="https://t.me/roboparty"><img src="https://img.shields.io/badge/Telegram-roboparty-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram: roboparty" height="24"></a>
  <a href="https://x.com/roboparty"><img src="https://img.shields.io/badge/X-%40roboparty-181818?style=flat-square&logo=x&logoColor=white" alt="X: @roboparty" height="24"></a>
  <a href="https://roboparty.com/wechat"><img src="https://img.shields.io/badge/WeChat-roboparty-07C160?style=flat-square&logo=wechat&logoColor=white" alt="WeChat: roboparty" height="24"></a>
  <a href="https://discord.gg/DTcW6rR3Xa"><img src="https://img.shields.io/badge/Discord-roboparty-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord: roboparty" height="24"></a>
  <a href="https://space.bilibili.com/3546938634930456"><img src="https://img.shields.io/badge/Bilibili-roboparty-00A1D6?style=flat-square&logo=bilibili&logoColor=white" alt="Bilibili: roboparty" height="24"></a>
</p>

<h3 align="center">The RoboParty Ecosystem</h3>

<p align="center">
  <a href="https://github.com/Roboparty/ROMOMO"><img src="assets/readme/romomo-card.jpg" alt="ROMOMO" width="32%"></a>
  <a href="https://github.com/Roboparty/Party_OS"><img src="https://opengraph.githubassets.com/1/Roboparty/Party_OS" alt="Party_OS" width="32%"></a>
  <a href="https://github.com/Roboparty/roboto_origin"><img src="https://opengraph.githubassets.com/f44bef10dbc6297cb05885961f85cf827ff0fce1ddd05ab08623bc02f79d338b/Roboparty/roboto_origin" alt="roboto_origin" width="32%"></a>
</p>

---

<p align="center">
  <strong>RoboParty</strong><br>
  Open hardware. Open intelligence. Shared possibility.
</p>

<p align="center">
  GPL-3.0 &nbsp; · &nbsp; © <a href="https://roboparty.com">RoboParty</a> &nbsp; · &nbsp; <a href="#top">Back to top</a><br>
  <sub>See each sub-repository for its applicable license.</sub>
</p>
