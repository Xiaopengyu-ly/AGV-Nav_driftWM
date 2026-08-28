# 结果图说明

以下结果由闭环评测与反事实推理性审计生成（本地复现，RTX 4060，seed 9000 × 50 场景）。

| 文件 | 内容 |
|---|---|
| `trajectories_grid_50scenarios_steps6.png` | 50 场景拼图：世界模型 MPPI（蓝实线）vs SAC 专家（灰虚线），叠在占用栅格上，标注起点/目标/到达/碰撞 |
| `traj_250000_arrived.png` | 场景 250000：MPPI 到达，SAC 失败（对比主图） |
| `traj_250002_arrived.png` | 场景 250002：到达（历史上曾失败的困难场景） |
| `traj_250010_collided.png` | 场景 250010：仍失败场景（4/50 之一） |
| `reasoning_audit_example_250010.png` | 反事实审计示例：MPPI 执行轨迹 + 决策点 + 同状态双开环推演（MPPI 所选 vs SAC 动作） |
