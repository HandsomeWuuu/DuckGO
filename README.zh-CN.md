# DuckGO

[English](README.md) | 中文

[![项目网站](assets/badge-website.svg)](http://43.156.246.20/?lang=zh)
[![Hugging Face 体验](assets/badge-huggingface.svg)](https://huggingface.co/spaces/HandsomeWu666/DuckGO)
![arXiv 论文待发布](assets/badge-arxiv.svg)

[![播放 DuckGO 障碍赛影片](assets/race-film-preview.gif)](http://43.156.246.20/showcase/duckgo-benchmark-review-10.mp4)

[观看完整影片（70 秒）](http://43.156.246.20/showcase/duckgo-benchmark-review-10.mp4)

**通用 Agent 能驾驶机器人跑完整场障碍赛吗？** 为了测试通用 Agent 的具身能力，我们在 MuJoCo 中设计了一场 Microduck 障碍赛。每个 Agent 驾驶一台双足机器人，通过相机画面和身体状态判断下一步，调用同一套运动技能，再根据实际走到的位置调整。Agent 思考时，赛道上的摆门仍在运动。

据我们所知，DuckGO 是首个让多个通用 Agent 调用同一套运动技能，各自实时驾驶机器人同场竞速的仿真障碍赛。赛道有 16 个检查点。单人试跑记录每个 Agent 独自能走多远。我们还让七个独立运行的 Agent 同时发车，在同一条赛道上竞速。对手可能挡住视线，一次碰撞也可能让机器人偏离原来的路线。

**比赛结果。** 15 场选定的单人试跑均未完赛。GPT-6 Astra 跑得最远，路线进度为 50.85%。DeepSeek V4.1 Flash 用 31 分 08 秒通过第 8 个检查点，Astra 用了 58 分 10 秒，两者都未通过第 9 个。在 V1 赛道的四组 Claude Code 配置中，Fable 5.1 通过 6 个检查点，Opus 5.5 通过 2 个。

## 体验 DuckGO

- [项目网站与成绩](http://43.156.246.20/?lang=zh)
- [Hugging Face Space 人工体验](https://huggingface.co/spaces/HandsomeWu666/DuckGO)：可用键盘或 Xbox 手柄控制 Microduck。目前需访问权限。

本仓库是 DuckGO 的公开项目主页。基准测试和 Agent 代码尚未在此发布。

## Microduck 相关项目与资源

- [Pollen Robotics · Microduck Sandbox](https://huggingface.co/spaces/pollen-robotics/microduck-simulator)：机器人仿真器。
- [Microduck Racer](https://huggingface.co/spaces/Nirav-Madhani/microduck-racer)：较早的 Microduck 竞赛环境。
- [microduck_rl](https://github.com/pollen-robotics/microduck_rl)：机器人强化学习环境。
- [Microduck policies](https://huggingface.co/pollen-robotics/microduck-policies)：训练得到的运动技能。
