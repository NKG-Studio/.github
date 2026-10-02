<h1 align="center">NKG Studio · NKG 工作室</h1>

<p align="center"><strong>AI 工作流 · 游戏开发 · 桌面效率工具</strong></p>
<p align="center">从 Agent 流程编排、游戏运行时与动画素材制作，到日常文件和大文本处理。<br />把开发中反复遇到的问题，做成可以直接使用和继续扩展的工具。</p>

<p align="center">
  <a href="#ai-工作流">AI 工作流</a> ·
  <a href="#游戏开发">游戏开发</a> ·
  <a href="#桌面工具">桌面工具</a> ·
  <a href="https://www.lfzxb.top">技术博客</a>
</p>

## 项目导航

| 你想做什么 | 项目 | 主要能力 |
| --- | --- | --- |
| 构建和运行 AI Agent 工作流 | [NKG AI Flow](https://github.com/NKG-Studio/nkg-ai-flow) | 可视化编排、运行调试、版本化热更新、多入口调用 |
| 开发可跨引擎复用的游戏逻辑 | [NKGGameFramework](https://github.com/NKG-Studio/NKGGameFramework) | 纯 .NET 核心、ECS、技能与 Buff、行为树、Web 调试 |
| 将视频制作成循环动画与游戏图集 | [FrameLoop Studio](https://github.com/NKG-Studio/nkg-ai-native-2d) | 循环分析、抠图精修、Sprite Sheet、MCP 自动化 |
| 统一组织多个目录和工程的文件 | [NKG 虚拟文件坞](https://github.com/NKG-Studio/nkg-folder) | 虚拟引用、多面板停靠、跨目录文件操作 |
| 阅读、搜索、编辑和对比大文本 | [NKG Uni Text Edit](https://github.com/NKG-Studio/nkg-uni-text-edit) | 按需读取、流式搜索、结构浏览、补丁式编辑 |

## AI 工作流

### NKG AI Flow

<p align="center">
  <a href="https://github.com/NKG-Studio/nkg-ai-flow"><img src="https://raw.githubusercontent.com/NKG-Studio/nkg-ai-flow/main/docs/assets/readme-cover.png" alt="NKG AI Flow" width="800" /></a>
</p>

**让 AI 参与工作流的构建与演进，让执行过程保持可控。**

面向 AI Agent 的可热更新 **Flow Runtime / Agent Harness**。通过 Flow Builder 或 Graph Operation 生成、修改和调试流程，结合 Studio 可视化编辑与运行事件追踪。

- 版本化发布：运行中的任务固定使用原版本，新任务使用新版本。
- 同一流程可通过 HTTP、CLI、MCP、SDK 和 Studio 调用。
- 提供节点扩展、流式输出、配置追踪，以及可选的运行审阅与干预能力。

[项目与安装说明 →](https://github.com/NKG-Studio/nkg-ai-flow)

## 游戏开发

### NKGGameFramework

**将游戏核心逻辑放在纯 C# 层，通过适配层连接具体引擎。**

基于 .NET 10 的引擎无关游戏框架。核心运行时、ECS 和玩法系统独立于具体宿主，Unity、Godot、Server 等通过 Adapter / Hosting 边界接入。

- 模块、事件、对象池、流程状态机与统一运行时上下文。
- ECS、GameplayTag、行为树、Skill / Buff 和通用节点图。
- 独立的 Diagnostics 与本地 Web Debug Host，支持运行态检查、快照录制与回放。
- 提供 AI 辅助游戏开发指南和示例工程。

<p align="center">
  <a href="https://github.com/NKG-Studio/NKGGameFramework"><img src="https://raw.githubusercontent.com/NKG-Studio/NKGGameFramework/main/pic/webdebug.png" alt="NKGGameFramework Web Debug Inspector" width="800" /></a>
</p>

[框架与接入说明 →](https://github.com/NKG-Studio/NKGGameFramework)

### FrameLoop Studio

**让 2D 动画自己找到完美循环。**

从视频抽帧、智能循环分析、抠图修边，到 Sprite Sheet 与引擎配套数据导出。可在浏览器中手动精修，也可通过本地 MCP 交给 AI 批量处理。

- 分析动作周期与首尾接缝，提供可解释的循环候选和可视化复核。
- 支持色度键、本地 AI 抠图、逐帧蒙版精修与非破坏时间线编辑。
- 导出图集及 Generic、Aseprite、Godot、Unity 数据预设，并提供独立 Sprite 切图。
- 浏览器端本地处理素材，MCP 支持分析、批量导出和结果校验。

<p align="center">
  <a href="https://github.com/NKG-Studio/nkg-ai-native-2d"><img src="https://raw.githubusercontent.com/NKG-Studio/nkg-ai-native-2d/main/docs/images/frameloop-studio-cover.png" alt="FrameLoop Studio 循环分析工作台" width="800" /></a>
</p>

[工作台与 MCP 使用说明 →](https://github.com/NKG-Studio/nkg-ai-native-2d)

## 桌面工具

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/NKG-Studio/nkg-folder"><img src="https://raw.githubusercontent.com/NKG-Studio/nkg-folder/main/assets/app-icon-master.png" alt="NKG Virtual Folder · VF" width="200" /></a>
      <h3>NKG 虚拟文件坞</h3>
      <p><strong>NKG Virtual Folder · VF</strong></p>
      <p>文件各在原处，工作尽在一处。</p>
      <p>面向多项目、多分支开发的 Windows 文件工作区。通过虚拟引用汇聚分散的目录和文件，结合多面板停靠、递归搜索与跨面板操作，减少目录之间的反复切换。</p>
      <p><a href="https://github.com/NKG-Studio/nkg-folder">查看项目与使用说明 →</a></p>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/NKG-Studio/nkg-uni-text-edit"><img src="https://raw.githubusercontent.com/NKG-Studio/nkg-uni-text-edit/main/crates/nkg-desktop/assets/nkg-icon-master.png" alt="NKG Uni Text Edit · UT" width="200" /></a>
      <h3>NKG Uni Text Edit</h3>
      <p><strong>大文本阅读、搜索、编辑与对比 · UT</strong></p>
      <p>按需读取，让大文件也能高效浏览。</p>
      <p>Rust 原生桌面工具，支持流式搜索、多组结果对比、JSON / XML 结构浏览和二进制模板解析。补丁式编辑可流式保存为新副本，适合日志分析与大文件排查。</p>
      <p><a href="https://github.com/NKG-Studio/nkg-uni-text-edit">查看项目与使用说明 →</a></p>
    </td>
  </tr>
</table>

## 使用与参与

安装方式、运行环境、当前支持范围和开发指南，以各项目 README 为准。遇到问题或有功能建议，欢迎在对应仓库提交 Issue；代码与文档改进欢迎通过 Pull Request 参与。

<p align="center">
  <a href="https://github.com/NKG-Studio?tab=repositories">浏览全部仓库</a> ·
  <a href="https://github.com/wqaetly">作者主页</a> ·
  <a href="https://www.lfzxb.top">技术博客</a>
</p>
