# YongQi Li · 李永祺

**[打开我的在线简历 → doribelove.github.io](https://doribelove.github.io/)**


电子科技大学（UESTC）在读学生，聚焦移动机器人导航、路径规划与系统工程。通过固定对照实验、边界测试和上游代码审阅持续验证工作。

Student at UESTC, working on mobile robotics, motion planning, and reliable software systems.

## Selected projects

- **[3YD / ROS 2 navigation workspace](https://github.com/Doribelove/pudu_robot_ws)** — 本地 r11 A+B 静态规划基线在固定集保持 **30/30** 严格成功，查询峰值 RSS 降低 **35.2%**，总体查询耗时中位数降低 **17.0%**。同环境对照；计时不含一次性准备及栈启动。公开仓库为较早快照。[实验摘要与边界](https://doribelove.github.io/evidence/3yd-v5-r11.md)。
- **[Autolabor Robot Navigation](https://github.com/Doribelove/autolabor-robot-nav)** — ROS Noetic 双机导航、FAST-LIO、覆盖规划、异步 Hybrid A* 与 TEB；**195 项工作区测试 + 10 项隔离生命周期测试通过**。完成 ARM64 构建与部署检查，该优化批次未进行实车运动性能验收。
- **[EGO-Planner on Ground](https://github.com/Doribelove/egoplanner_on_ground)** — 地面车二维规划、B 样条轨迹、MPC 控制与点云预处理的适配实践。

## Accepted open-source contributions

**7 pull requests merged into 6 external upstream projects**, verified on **2026-09-22**. Merges into my own repositories are not included.

| Project | Merged contribution |
| --- | --- |
| [Sparse #963](https://github.com/pydata/sparse/pull/963) | Preserve zero-dimensional arrays in COO / DOK construction and conversion |
| [Sparse #957](https://github.com/pydata/sparse/pull/957) | Avoid dense column-selector allocation in GCXS basic slicing |
| [Robotics Toolbox #669](https://github.com/petercorke/robotics-toolbox-python/pull/669) | Preserve joint types and limits in numerical inverse kinematics |
| [pytransform3d #373](https://github.com/dfki-ric/pytransform3d/pull/373) | Fix batch axis-angle conversion and output allocation |
| [Trimesh #2600](https://github.com/mikedh/trimesh/pull/2600) | Correct the principal angle returned by vector alignment |
| [Gymnasium #1694](https://github.com/Farama-Foundation/Gymnasium/pull/1694) | Require matching Tuple lengths in space compatibility checks |
| [PettingZoo #1457](https://github.com/Farama-Foundation/PettingZoo/pull/1457) | Avoid overflow when rescaling wide finite float64 observation bounds |

**In review:** [Sparse #962](https://github.com/pydata/sparse/pull/962) adds sparse boolean masks to COO / GCXS indexing. Updated following review; 243 targeted tests and the GitHub Numba Array API check pass. **Not merged** as of the date above.

[View all open pull requests](https://github.com/pulls?q=is%3Apr+is%3Aopen+author%3ADoribelove).

## Technical focus

C++ / Python · ROS 1 / ROS 2 · Nav2 · FAST-LIO / ICP · Hybrid A* / TEB · B-spline / MPC · Linux · automated testing and performance analysis.

## Open-source communities

- **[FOSSASIA](https://github.com/fossasia)** — public GitHub organization member. [Membership](https://github.com/orgs/fossasia/people?query=Doribelove)
- **[Your First Open Source Project (YFOSP)](https://github.com/yfosp)** — public GitHub organization member. [Membership](https://github.com/orgs/yfosp/people?query=Doribelove)

[View GitHub achievements](https://github.com/Doribelove?tab=achievements).

Some implementation, tests, and documentation used AI assistance. Results are based on recorded experiments, executed validation, and upstream merge records; local tests, review approval, and merging are distinct outcomes.
