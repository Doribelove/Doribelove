# YongQi Li

电子科技大学本硕，关注 **移动机器人、智能驾驶、物理AI与多模态检索问答**。开展算法实现、系统集成与实车验证，持续向机器人与科学计算开源项目贡献修复。

[在线简历](https://doribelove.github.io/) · [可打印简历](https://doribelove.github.io/resume/) · [项目图文与视频](https://doribelove.github.io/projects/) · [联系邮箱](mailto:doribelove@gmail.com)

## 论文成果

**SDERI: Autonomous Navigation with Safe Subgoal Distributions and Exploration-Replanning Index in Dynamic Environments**  
IROS 2026 · Paper **775** · **学生第二作者**  

围绕动态环境自主导航，研究安全子目标分布与探索—重规划决策。
[官方论文入口与摘要](https://2026.ieee-iros.org/program/contributed_talks/#eeb7f7:775) · [官方作者索引](https://2026.ieee-iros.org/program/paper-index/?q=SDERI) · [作者项目与演示视频](https://sites.google.com/view/sderifornavigation)

**通航机场动态环境下无人车路径规划方法**  
《系统工程与电子技术》· **第一作者** · **已录用，待发表（预计 2026 年 11 月）**  

结合改进 Hybrid A* 与优化 TEB，引入 Reeds–Shepp 回溯、加加速度约束和级联 PID 跟踪校正，研究机场动态环境下的路径平滑性、避障与运动稳定性，并进行仿真与实物验证。
[作者稿 PDF](https://doribelove.github.io/papers/ssee-2026-1172-author-manuscript.pdf) · [论文详情](https://doribelove.github.io/#publications)

## 核心完整项目

### [普渡 · 分层导航与运动规划](https://github.com/Doribelove/pudu_robot_ws)

基于 ROS 2 / Nav2 构建分层规划链路，连接拓扑引导、参考路径、运动学搜索与轨迹校验，完成大地图规划、性能优化和可视化。V11-r3 静态规划测试共 300 次，297 次精确到达、3 次容差到达；请求耗时中位数 **0.816 s**、P95 **3.657 s**。
[图文与实验结果](https://doribelove.github.io/projects/#pudu) · [项目源码](https://github.com/Doribelove/pudu_robot_ws)

### [净途智行 · 国产无人清扫车系统](https://github.com/Doribelove/autolabor-robot-nav/tree/robot_j6m_ws)

地平线挑战杯项目负责人，基于 **J6M + Jetson AGX** 构建定位、感知、规划、交互与清扫执行系统。J6M 承担定位建图、覆盖规划、局部避障和控制仲裁，AGX 承担模型推理、语音解析与 Qt 交互。集成 FAST-LIO / ICP 或双天线 GNSS、Hybrid A* / TEB、三路环视垃圾识别与 BEV 坐标映射，并通过 **Qwen 8B** 解析和分解清扫任务。

围绕斑马线减速、靠右行驶、信号灯响应，以及工厂、地下停车场和商场覆盖规划，提供三维场景演示。在机场场景完成 **160 m² 导航覆盖**、覆盖率 **98.0%**。2026 年 10 月重新装配车辆，在机坪和滑行道开展黎明、白天、黄昏与夜晚测试，取得 **24 次回收成功、12 次避障成功**，提供实车演示与轨迹、相机、点云同步回放。
[完整项目与视频演示](https://doribelove.github.io/projects/#autolabor) · [robot_j6m_ws 源码](https://github.com/Doribelove/autolabor-robot-nav/tree/robot_j6m_ws)

### [多旋翼无人机 · 自主导航与视觉抓取](https://doribelove.github.io/projects/#drone)

负责飞行平台设计与系统集成，并担任自主抓取项目队长。完成四旋翼结构、动力与供电设计，基于 **PX4 / MAVROS / Jetson / ROS** 连接飞控、机载感知与任务执行，平台有效载荷 **>1.5 kg**、续航 **>20 min**。

修改并部署 **EGO-Planner**，结合 **YOLOv8 与视觉伺服**完成障碍环境导航、柱面 QR 码识别、目标靠近、机械抓取与定点投放。获 **2024 年第四届四川省大学生未来飞行器挑战赛实践类一等奖**，完成“科研育人”翱翔计划 **优秀 A 结题**。
[项目图文与演示](https://doribelove.github.io/projects/#drone) · [实机测试：目标识别与悬停](https://doribelove.github.io/projects/#drone-field)

### [魔方机器人 · 双臂视觉复原](https://github.com/Doribelove/robot_mofang)

基于四路视觉识别、**Two-Phase** 求解与双臂协同执行，完成从六面图像采集、54 位状态识别、复原公式计算到机械动作优化的完整系统。使用 **ODrive + Arduino** 控制双腕与夹爪，**7 秒完成识别、解算和成功还原**。获 **2024 年第七届中国高校智能机器人创意大赛国家级二等奖**，总排名 **9/55**。
[实物图集](https://doribelove.github.io/projects/#cube-gallery) · [实机测试视频](https://doribelove.github.io/projects/#cube-tests) · [项目与完整视频](https://doribelove.github.io/projects/#cube) · [项目源码](https://github.com/Doribelove/robot_mofang) · [B 站演示](https://www.bilibili.com/video/BV1haNg6fE5s/)

### [不二鸟 · 华为存储杯多模态检索问答](https://github.com/Doribelove/huawei-storage-cup-mrag)

面向 PDF 文本、表格与图像，以 **BGE-M3 + BGE reranker + Qwen3-VL-8B** 构建检索、Reader、来源绑定和证据支持检查，支持本地建库与 question-only HTTP 查询，并实现基于证据充分性的拒答处理。

30 题本地评测中，同模型判分 **26/30**，作者对照原文审阅的完整支持结果为 **25/30**。
[图文与案例](https://doribelove.github.io/projects/#huawei) · [系统设计](https://github.com/Doribelove/huawei-storage-cup-mrag/blob/main/docs/DESIGN.md)

## 开源贡献

截至 **2026-10-27**，**26 个 PR 已合并至 11 个上游开源项目**。

| 项目 | 近期或代表性贡献 | 合并记录 |
| --- | --- | --- |
| REA | 修复 Mach-O 动态库路径解析，保留换行符与 Unicode 行分隔符 | [#5363](https://github.com/morluto/rea/pull/5363) |
| Robotics Toolbox | 补全 mstraj 轨迹速度、加速度与时间轨迹标记 | [#706](https://github.com/petercorke/robotics-toolbox-python/pull/706) |
| SpatialMath | 修复三维直线关系的尺度敏感问题、直线距离计算与 Python 3.10 Self 依赖 | [#232](https://github.com/rai-opensource/spatialmath-python/pull/232) · [#224](https://github.com/rai-opensource/spatialmath-python/pull/224) · [#233](https://github.com/rai-opensource/spatialmath-python/pull/233) |
| Pint | 按函数签名处理可变位置参数的单位换算 | [#2422](https://github.com/hgrecco/pint/pull/2422) |
| PyData / Sparse | 稀疏切片内存优化、零维数组转换、列优先 flatten | [#957](https://github.com/pydata/sparse/pull/957) · [#963](https://github.com/pydata/sparse/pull/963) · [#964](https://github.com/pydata/sparse/pull/964) |
| GitHub / Spec Kit | 扩展历史版本查询与精确版本安装 | [#4726](https://github.com/github/spec-kit/pull/4726) |
| Gymnasium / PettingZoo | 整数空间批处理；Parallel API 动作裁剪支持 | [#1695](https://github.com/Farama-Foundation/Gymnasium/pull/1695) · [#1489](https://github.com/Farama-Foundation/PettingZoo/pull/1489) |

[查看全部上游合并记录](https://github.com/search?q=is%3Apr+is%3Amerged+author%3ADoribelove+-user%3ADoribelove&type=pullrequests) · [26 项贡献详情](https://doribelove.github.io/evidence/contributions-20261027.json)

## 更多实践与技术栈

[EGO-Planner 地面车适配](https://github.com/Doribelove/egoplanner_on_ground) · [覆盖导航](https://github.com/Doribelove/autolabor-coverage-navigation) · [Qt 机器人操作界面](https://github.com/Doribelove/QT-UI) · [魔方机器人](https://github.com/Doribelove/robot_mofang) · [AIFS 分布式文件系统](https://github.com/Doribelove/AIFS) · [贡献报告工具](https://github.com/Doribelove/github-contribution-report)

**C++ / Python · ROS 1 / ROS 2 · Linux · Nav2 · FAST-LIO / ICP · Hybrid A* / TEB · B-spline / MPC · 多模态 RAG**

更新于 2026-10-28。
