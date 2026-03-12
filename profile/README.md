# CheckScopeHyzc

面向 C/C++ 工程代码的静态分析、源码取证与可追溯智能确认组织。

## 我们在做什么

- 构建源码级调用关系、符号索引与证据回放能力
- 融合规则体系与大模型能力进行缺陷确认
- 产出结构化、可审计、可复现的确认结果
- 沉淀评测、试运行和规则验证闭环

## 核心项目

- [CheckScopeAIAgent](https://github.com/CheckScopeHyzc/CheckScopeAIAgent)：基于 Django / DRF / Celery / PostgreSQL 的静态缺陷确认系统，覆盖任务编排、证据包构建、模型适配、评测与试运行闭环。
- [SourceTrace](https://github.com/CheckScopeHyzc/SourceTrace)：源码解析、符号索引、调用关系与源码取证能力参考实现。
- [CheckScopeAI](https://github.com/CheckScopeHyzc/CheckScopeAI)：规则 + LLM 静态分析确认框架与历史能力沉淀。

## 当前能力基线

- 支持 `GJB8114`、`CWE` 与自定义规则导入
- 支持 `Doxygen + compile_commands.json` 驱动的源码解析增强
- 支持本地 OpenAI-compatible 模型适配与结构化输出校验
- 支持规则级评测、回归基线、试运行问题台账与阈值微调
- 支持 Docker 化部署与 PostgreSQL 17.9 持久化基线

## 目标

- 提升静态分析结果确认效率
- 降低人工复核与追溯成本
- 支持团队化持续集成、试运行与验收落地
