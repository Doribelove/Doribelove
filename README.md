# 李永祺 · YongQi Li

电子科技大学在读，关注 **移动机器人导航、运动规划与多模态检索问答**。从算法实现、系统集成到实车记录，持续向机器人与科学计算开源项目贡献修复。

[在线简历](https://doribelove.github.io/) · [可打印简历](https://doribelove.github.io/resume/) · [项目图文与视频](https://doribelove.github.io/projects/) · [联系邮箱](mailto:doribelove@gmail.com)

## 论文成果

**SDERI: Autonomous Navigation with Safe Subgoal Distributions and Exploration-Replanning Index in Dynamic Environments**  
IROS 2026 · Paper **775** · **学生第二作者（总作者排序第三）**  
Jingru Zhang, Mingzhu Wei, **Yongqi Li**, Zhenni Zeng, Min Gong, Hui Li.

围绕动态环境自主导航，研究安全子目标分布与探索—重规划决策。
[官方论文入口与摘要](https://2026.ieee-iros.org/program/contributed_talks/#eeb7f7:775) · [官方作者索引](https://2026.ieee-iros.org/program/paper-index/?q=SDERI) · [作者项目与演示视频](https://sites.google.com/view/sderifornavigation)

**通航机场动态环境下无人车路径规划方法**  
《系统工程与电子技术》· **第一作者** · **已录用，待发表（预计 2026 年 11 月）**  
**李永祺**，魏明珠，曾珍妮，张景茹，李辉，龚敏，董巾航。

结合改进 Hybrid A* 与优化 TEB，引入 Reeds–Shepp 回溯、加加速度约束和级联 PID 跟踪校正，研究机场动态环境下的路径平滑性、避障与运动稳定性，并进行仿真与实物验证。
[作者稿 PDF](https://doribelove.github.io/papers/ssee-2026-1172-author-manuscript.pdf) · [论文详情](https://doribelove.github.io/#publications)

## 近期项目

### [普渡 · 分层导航与运动规划](https://github.com/Doribelove/pudu_robot_ws)

ROS 2 / Nav2 工作实践：连接拓扑引导、参考路径、运动学搜索和终验，整理大地图规划结果、性能记录与可视化。最新公开 V11-r3 静态完整规划记录：300 次中 297 次精确到达、3 次容差到达，均满足该版验收规则；耗时中位 **0.816 s**、P95 **3.657 s**。范围为静态实验和指定受控事件回放，实车验收另计。
[图文与实验入口](https://doribelove.github.io/projects/#pudu) · [源码与最新记录](https://github.com/Doribelove/pudu_robot_ws)

### [净途智行 · 地平线挑战杯实车项目](https://github.com/Doribelove/autolabor-robot-nav/tree/robot_j6m_ws)

J6M + Jetson 双机无人清扫车，集成 FAST-LIO / ICP 或双天线 GNSS、条带覆盖、Hybrid A*、TEB、YOLO11s-GAM 以及语音 / Qt 任务交互。技术报告记录了 **160 m² / 98.0% 导航覆盖**；另有安装清扫机构后的实际刷扫与垃圾收集视频。
[实车照片与视频](https://doribelove.github.io/projects/#autolabor) · [robot_j6m_ws 源码](https://github.com/Doribelove/autolabor-robot-nav/tree/robot_j6m_ws)

### [不二鸟 · 华为存储杯多模态检索问答](https://github.com/Doribelove/huawei-storage-cup-mrag)

面向 PDF 文本、表格与图像，以 **BGE-M3 + BGE reranker + Qwen3-VL-8B** 构建检索、Reader、来源绑定和证据支持检查，适配本地建库与 question-only HTTP 查询。公开 r58 已提交版本源码、真实输入输出及拒答案例。

历史 30 题开发集：本地同模型判分 **26/30**，同作者原文完整支持审阅 **25/30**；属于开发记录，不作为官方比赛成绩。
[图文与案例](https://doribelove.github.io/projects/#huawei) · [系统设计](https://github.com/Doribelove/huawei-storage-cup-mrag/blob/main/docs/DESIGN.md)

## 开源贡献

截至 **2026-10-16**，**24 个 PR 已合并至 10 个其他所有者的上游仓库**，不含自有仓库内部合并。

| 项目 | 近期或代表性贡献 | 合并记录 |
| --- | --- | --- |
| Robotics Toolbox | 补全 mstraj 轨迹速度、加速度与时间轨迹标记 | [#706](https://github.com/petercorke/robotics-toolbox-python/pull/706) |
| SpatialMath | Python 3.10 Self 依赖修复；三维直线距离计算修复 | [#233](https://github.com/rai-opensource/spatialmath-python/pull/233) · [#224](https://github.com/rai-opensource/spatialmath-python/pull/224) |
| Pint | 按函数签名处理可变位置参数的单位换算 | [#2422](https://github.com/hgrecco/pint/pull/2422) |
| PyData / Sparse | 稀疏切片内存优化、零维数组转换、列优先 flatten | [#957](https://github.com/pydata/sparse/pull/957) · [#963](https://github.com/pydata/sparse/pull/963) · [#964](https://github.com/pydata/sparse/pull/964) |
| GitHub / Spec Kit | 扩展历史版本查询与精确版本安装 | [#4726](https://github.com/github/spec-kit/pull/4726) |
| Gymnasium / PettingZoo | 整数空间批处理；Parallel API 动作裁剪支持 | [#1695](https://github.com/Farama-Foundation/Gymnasium/pull/1695) · [#1489](https://github.com/Farama-Foundation/PettingZoo/pull/1489) |

[查看全部上游合并记录](https://github.com/search?q=is%3Apr+is%3Amerged+author%3ADoribelove+-user%3ADoribelove&type=pullrequests) · [24 项核验清单](https://doribelove.github.io/evidence/contributions-20261016.json)

## 更多实践与技术栈

[EGO-Planner 地面车适配](https://github.com/Doribelove/egoplanner_on_ground) · [覆盖导航](https://github.com/Doribelove/autolabor-coverage-navigation) · [Qt 机器人操作界面](https://github.com/Doribelove/QT-UI) · [魔方机器人](https://github.com/Doribelove/robot_mofang) · [AIFS 分布式文件系统](https://github.com/Doribelove/AIFS) · [贡献报告工具](https://github.com/Doribelove/github-contribution-report)

**C++ / Python · ROS 1 / ROS 2 · Linux · Nav2 · FAST-LIO / ICP · Hybrid A* / TEB · B-spline / MPC · 多模态 RAG**

更新于 2026-10-16。论文发表预期以期刊最终安排为准；项目指标均附对应记录与适用范围。
