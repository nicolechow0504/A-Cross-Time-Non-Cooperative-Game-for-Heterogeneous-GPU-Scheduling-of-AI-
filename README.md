# A-Cross-Time-Non-Cooperative-Game-for-Heterogeneous-GPU-Scheduling-of-AI-
This is my personal thesis display library.
Alibaba GPU Trace 跨时段博弈研究展示网站（离线版）
=================================================

打开方式
1. 解压压缩包，并保持 index.html、styles.css、app.js 与 assets 文件夹的相对位置不变。
2. 双击 index.html，即可在 Chrome、Edge、Firefox 或 Safari 中离线运行。
3. 网站不使用 CDN、在线字体、远程接口或后端服务。

答辩操作
- 按 F 或点击右上角“答辩模式”进入章节演示。
- 答辩模式下使用 ← / → 切换章节，Esc 退出。
- 点击“三分钟答辩导览”可快速串联问题、方法、结果与反思。
- 数据区可切换总需求、高性能 GPU、成本与迁出需求时序。
- 关键图表可点击放大；右上角 ⇩ 可打印或导出 PDF。

真实性说明
- 数据、参数、结果与关键图表均来自随附 GPU_game最终 工程。
- “复盘与反思”依据 prepare_gpu_game_data.py、game_model.py、
  run_time_series_experiment.py、实验 CSV 与论文限制段落整理。
- 网站明确呈现负面结果，包括成本上升、基础资源波动上升、参数敏感性缺失、
  物理容量约束缺失以及默认参数不一致。

关键实验口径
- Alibaba Cluster Trace GPU v2020
- Top 2–31 高需求用户，N=30；排除最大用户
- 30 个非零日粒度时隙
- movable fraction φ=0.50；maximum delay D=2 bins
- shift penalty ρ=2.0；smooth penalty η=1.0；price weight=0.70
- 主实验实际使用 lambda_high=0.02、lambda_basic=0.0012

文件结构
- index.html：页面结构与学术叙事
- styles.css：视觉、响应式与打印样式
- app.js：真实时序数据、交互图表与答辩逻辑
- assets/：论文实验原图

