# DuckGO

![DuckGO obstacle course](assets/cover.jpg)

**Can a general-purpose agent guide a physically simulated robot through an entire obstacle race using only first-person visual observations?**

DuckGO studies an agent as the embodied decision-maker for Microduck, a biped robot in a MuJoCo obstacle course. The agent selects from available movement skills, observes what actually happened, and decides again. Skill outcomes are not guaranteed, and in real-time runs the environment continues to change while the agent thinks.

The course has 16 ordered stages, including narrow passages, moving gates, shifting barriers, low bars, and other obstacles. Results are organized by solo versus simultaneous races, with real-time and paused-inference settings kept separate.

## Explore DuckGO

- [Project website and results](http://43.156.246.20/showcase.html?lang=en)
- [Play on Hugging Face Spaces](https://huggingface.co/spaces/HandsomeWu666/DuckGO) — drive Microduck with a keyboard or Xbox controller. The Space currently requires access permission.

This repository is the public project landing page. Benchmark and agent code are not published here yet.

## Projects and references

**Microduck ecosystem**

- [Pollen Robotics · Microduck Sandbox](https://huggingface.co/spaces/pollen-robotics/microduck-simulator) — robot simulator.
- [Microduck Racer](https://huggingface.co/spaces/Nirav-Madhani/microduck-racer) — earlier Microduck racing environment.
- [microduck_rl](https://github.com/pollen-robotics/microduck_rl) — robot reinforcement-learning environments.
- [Microduck policies](https://huggingface.co/pollen-robotics/microduck-policies) — learned motion skills.

**Evaluation context**

- [GameWorld](https://gameworld-project.github.io/) — standardized, verifiable evaluation of multimodal game agents.
- [GameHorizon Suite](https://gamehorizon-suite.github.io/) — multi-horizon gameplay data and evaluation.

DuckGO uses a physically simulated robot and tests the agent's repeated decisions after uncertain skill execution; the two game-agent projects above are research context, not components of the simulator.

---

## 中文简介

DuckGO 研究通用 Agent 能否仅凭第一视角画面，持续控制物理仿真的双足机器人 Microduck 完成整场障碍赛。Agent 从给定技能中选择动作，再根据实际执行结果重新观察和决策；技能不保证成功，实时模式下仿真也不会等待模型思考。

赛道包含 16 个有序关卡。成绩按单鸭与多鸭同场、实时与推理暂停分别展示。[项目网站](http://43.156.246.20/showcase.html?lang=zh)提供赛道、实验设置和结果；[Hugging Face Space](https://huggingface.co/spaces/HandsomeWu666/DuckGO) 提供键盘或 Xbox 手柄的人工体验入口（目前需访问权限）。参考项目及其与 DuckGO 的关系见上方链接。本仓库目前只公开项目介绍与封面，暂不包含测试代码。
