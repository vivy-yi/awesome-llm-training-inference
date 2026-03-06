# Awesome LLM 训练与推理

> 精选的 LLM 训练与推理框架、工具和资源列表。涵盖从数据处理到部署的完整流程。

[![License](https://img.shields.io/badge/license-CC0--1.0-blue)](LICENSE)

[English](README.md) | 简体中文

<!-- keywords: LLM, 大语言模型, 训练, 推理, 深度学习, 机器学习, PyTorch, transformers, 分布式训练, 模型服务 -->

## 目录

- [训练框架](#训练框架)
- [预训练实现](#预训练实现)
- [端到端训练与推理](#端到端训练与推理)
- [推理框架](#推理框架)
- [分布式训练](#分布式训练)
- [硬件加速](#硬件加速)
- [微调与 PEFT](#微调与-peft)
- [模型压缩与量化](#模型压缩与量化)
- [数据工程](#数据工程)
- [隐私与安全](#隐私与安全)
- [垂直领域 LLM](#垂直领域-llm)
- [RAG 与向量搜索](#rag-与向量搜索)
- [评估与基准](#评估与基准)
- [科研工具](#科研工具)
- [MLOps 与平台](#mlops-与平台)
- [部署与服务](#部署与服务)
- [监控与可观测性](#监控与可观测性)
- [学习资源](#学习资源)
- [贡献指南](#贡献指南)
- [许可证](#许可证)

---

## 训练框架

### 深度学习框架

| 框架 | Stars | 描述 |
|------|-------|------|
| [PyTorch](https://github.com/pytorch/pytorch) | ![Stars](https://img.shields.io/github/stars/pytorch/pytorch) | 开源机器学习框架 |
| [transformers](https://github.com/huggingface/transformers) | ![Stars](https://img.shields.io/github/stars/huggingface/transformers) | 先进的文本、视觉、音频 ML 框架 |
| [JAX](https://github.com/google/jax) | ![Stars](https://img.shields.io/github/stars/google/jax) | ML 可组合转换框架 |
| [Flax](https://github.com/google/flax) | ![Stars](https://img.shields.io/github/stars/google/flax) | 基于 JAX 的神经网络库 |

### 训练库

| 框架 | Stars | 描述 |
|------|-------|------|
| [Accelerate](https://github.com/huggingface/accelerate) | ![Stars](https://img.shields.io/github/stars/huggingface/accelerate) | PyTorch 分布式训练简化工具 |
| [Lightning](https://github.com/Lightning-AI/pytorch-lightning) | ![Stars](https://img.shields.io/github/stars/Lightning-AI/pytorch-lightning) | 可扩展训练的深度学习框架 |
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/deepspeedai/DeepSpeed) | 深度学习优化库 |
| [Fairscale](https://github.com/facebookresearch/fairscale) | ![Stars](https://img.shields.io/github/stars/facebookresearch/fairscale) | PyTorch 高性能训练扩展 |

---

## 预训练实现

### 从零开始实现

| 框架 | Stars | 描述 |
|------|-------|------|
| [nanoGPT](https://github.com/karpathy/nanoGPT) | ![Stars](https://img.shields.io/github/stars/karpathy/nanoGPT) | Karpathy 的最小 GPT-2 训练实现 |
| [lit-llama](https://github.com/Lightning-AI/lit-llama) | ![Stars](https://img.shields.io/github/stars/Lightning-AI/lit-llama) | 基于 nanoGPT 的 LLaMA 实现 |
| [GPT-NeoX](https://github.com/EleutherAI/gpt-neox) | ![Stars](https://img.shields.io/github/stars/EleutherAI/gpt-neox) | 大规模自回归 Transformers |
| [lunariscodex](https://github.com/MeryylleA/lunariscodex) | ![Stars](https://img.shields.io/github/stars/MeryylleA/lunariscodex) | 高性能 Llama 风格预训练工具包 |

---

## 端到端训练与推理

### 端到端微调

| 框架 | Stars | 描述 |
|------|-------|------|
| [Axolotl](https://github.com/axolotl-ai/axolotl) | ![Stars](https://img.shields.io/github/stars/axolotl-ai/axolotl) | 用户友好的 LLM 微调工具 |
| [LlamaFactory](https://github.com/hiyouga/LlamaFactory) | ![Stars](https://img.shields.io/github/stars/hiyouga/LlamaFactory) | 统一高效微调 100+ LLM |
| [xturing](https://github.com/stochasticai/xTuring) | ![Stars](https://img.shields.io/github/stars/stochasticai/xTuring) | 构建、个性化和控制自己的 LLM |

### 端到端推理

| 框架 | Stars | 描述 |
|------|-------|------|
| [vLLM](https://github.com/vllm-project/vllm) | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm) | 高吞吐量 LLM 推理引擎 |
| [Ollama](https://github.com/ollama/ollama) | ![Stars](https://img.shields.io/github/stars/ollama/ollama) | 本地运行 LLM |
| [SGLang](https://github.com/sgl-project/sglang) | ![Stars](https://img.shields.io/github/stars/sgl-project/sglang) | 高性能 LLM 服务框架 |

---

## 推理框架

### 高性能推理

| 框架 | Stars | 描述 |
|------|-------|------|
| [vLLM](https://github.com/vllm-project/vllm) | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm) | 高吞吐量 LLM 推理引擎 |
| [SGLang](https://github.com/sgl-project/sglang) | ![Stars](https://img.shields.io/github/stars/sgl-project/sglang) | 高性能 LLM 服务框架 |
| [Text Generation Inference](https://github.com/huggingface/text-generation-inference) | ![Stars](https://img.shields.io/github/stars/huggingface/text-generation-inference) | Hugging Face 生产级推理服务器 |
| [LightLLM](https://github.com/ModelTC/LightLLM) | ![Stars](https://img.shields.io/github/stars/ModelTC/LightLLM) | 轻量级 LLM 推理框架 |
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | ![Stars](https://img.shields.io/github/stars/ggerganov/llama.cpp) | C/C++ LLM 推理 |
| [Ollama](https://github.com/ollama/ollama) | ![Stars](https://img.shields.io/github/stars/ollama/ollama) | 本地运行 LLM |

### 本地与边缘推理

| 框架 | Stars | 描述 |
|------|-------|------|
| [LM Studio](https://github.com/lmstudio-ai/lmstudio) | ![Stars](https://img.shields.io/github/stars/lmstudio-ai/lmstudio) | 发现并运行本地 LLM |
| [IPEX-LLM](https://github.com/intel/ipex-llm) | ![Stars](https://img.shields.io/github/stars/intel/ipex-llm) | Intel 硬件上的 LLM 推理加速 |
| [llamafile](https://github.com/Mozilla-Ocho/llamafile) | ![Stars](https://img.shields.io/github/stars/Mozilla-Ocho/llamafile) | 单文件可执行 LLM |

### 多 LoRA 服务

| 框架 | Stars | 描述 |
|------|-------|------|
| [LoRAX](https://github.com/predibase/lorax) | ![Stars](https://img.shields.io/github/stars/predibase/lorax) | 多租户 LoRA 服务框架 |
| [fastapi-lora](https://github.com/lm-sys/fastapi-lora) | ![Stars](https://img.shields.io/github/stars/lm-sys/fastapi-lora) | 快速 LoRA 推理服务 |

---

## 分布式训练

### 并行训练框架

| 框架 | Stars | 描述 |
|------|-------|------|
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/deepspeedai/DeepSpeed) | ZeRO 优化的分布式训练 |
| [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | ![Stars](https://img.shields.io/github/stars/NVIDIA/Megatron-LM) | 大规模 Transformer 训练 |
| [ColossalAI](https://github.com/hpcaitech/ColossalAI) | ![Stars](https://img.shields.io/github/stars/hpcaitech/ColossalAI) | 大规模模型训练系统 |

### 训练优化

| 框架 | Stars | 描述 |
|------|-------|------|
| [FlashAttention](https://github.com/Dao-AILab/flash-attention) | ![Stars](https://img.shields.io/github/stars/Dao-AILab/flash-attention) | 快速且内存高效的注意力机制 |
| [xFormers](https://github.com/facebookresearch/xformers) | ![Stars](https://img.shields.io/github/stars/facebookresearch/xformers) | Transformer 模块化组件 |

---

## 硬件加速

| 框架 | Stars | 描述 |
|------|-------|------|
| [IPEX-LLM](https://github.com/intel/ipex-llm) | ![Stars](https://img.shields.io/github/stars/intel/ipex-llm) | Intel GPU/CPU 上的 LLM 推理加速 |
| [OpenVINO](https://github.com/openvinotoolkit/openvino) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/openvino) | Intel 硬件推理优化工具包 |
| [Triton](https://github.com/triton-inference-server/triton) | ![Stars](https://img.shields.io/github/stars/triton-inference-server/triton) | 开源 GPU 推理服务器 |

---

## 微调与 PEFT

### 参数高效微调

| 框架 | Stars | 描述 |
|------|-------|------|
| [PEFT](https://github.com/huggingface/peft) | ![Stars](https://img.shields.io/github/stars/huggingface/peft) | 先进的参数高效微调 |
| [LlamaFactory](https://github.com/hiyouga/LlamaFactory) | ![Stars](https://img.shields.io/github/stars/hiyouga/LlamaFactory) | 统一高效微调 100+ LLM |
| [xTuring](https://github.com/stochasticai/xTuring) | ![Stars](https://img.shields.io/github/stars/stochasticai/xTuring) | 构建、个性化和控制自己的 LLM |
| [Unsloth](https://github.com/unslothai/unsloth) | ![Stars](https://img.shields.io/github/stars/unslothai/unsloth) | 内存高效微调 (2倍快，70%更少内存) |
| [ArcticTraining](https://github.com/snowflakedb/ArcticTraining) | ![Stars](https://img.shields.io/github/stars/snowflakedb/ArcticTraining) | Snowflake 的 LLM 后训练框架 |
| [SteptronOss](https://github.com/stepfun-ai/SteptronOss) | ![Stars](https://img.shields.io/github/stars/stepfun-ai/SteptronOss) | 轻量级 AI 原生 LLM 训练框架 |

### RLHF 与对齐

| 框架 | Stars | 描述 |
|------|-------|------|
| [TRL](https://github.com/huggingface/trl) | ![Stars](https://img.shields.io/github/stars/huggingface/trl) | 使用 RLHF 和 DPO 训练语言模型 |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/microsoft/DeepSpeed) | 易用的 RLHF 训练流水线 |

---

## 模型压缩与量化

### 量化工具

| 框架 | Stars | 描述 |
|------|-------|------|
| [BitsAndBytes](https://github.com/TimDettmers/bitsandbytes) | ![Stars](https://img.shields.io/github/stars/TimDettmers/bitsandbytes) | LLM 8-bit 量化 |
| [AWQ](https://github.com/mit-han-lab/awq) | ![Stars](https://img.shields.io/github/stars/mit-han-lab/awq) | 激活感知权重量化 |
| [GPTQ](https://github.com/IST-DASLab/gptq) | ![Stars](https://img.shields.io/github/stars/IST-DASLab/gptq) | GPT 后训练量化 |
| [GGML](https://github.com/ggerganov/ggml) | ![Stars](https://img.shields.io/github/stars/ggerganov/ggml) | ML 张量库 |
| [exllamav2](https://github.com/turboderp-org/exllamav2) | ![Stars](https://img.shields.io/github/stars/turboderp-org/exllamav2) | 在消费级 GPU 上运行 LLM 的优化量化 |

### 压缩框架

| 框架 | Stars | 描述 |
|------|-------|------|
| [NNCF](https://github.com/openvinotoolkit/nncf) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/nncf) | 神经网络压缩框架 |
| [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | ![Stars](https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM) | NVIDIA LLM 推理优化 |
| [Optimum](https://github.com/huggingface/optimum) | ![Stars](https://img.shields.io/github/stars/huggingface/optimum) | Transformers 优化工具 |
| [Model-Optimizer](https://github.com/NVIDIA/Model-Optimizer) | ![Stars](https://img.shields.io/github/stars/NVIDIA/Model-Optimizer) | 统一 SOTA 模型优化技术 (量化、剪枝、知识蒸馏) |

---

## 数据工程

### 数据处理

| 框架 | Stars | 描述 |
|------|-------|------|
| [DataLoader](https://github.com/pytorch/data) | ![Stars](https://img.shields.io/github/stars/pytorch/data) | PyTorch 数据加载工具 |
| [Datasets](https://github.com/huggingface/datasets) | ![Stars](https://img.shields.io/github/stars/huggingface/datasets) | ML 公共数据集 |
| [WebDataset](https://github.com/webdataset/webdataset) | ![Stars](https://img.shields.io/github/stars/webdataset/webdataset) | 大规模数据集处理 |
| [PyArrow](https://github.com/apache/arrow) | ![Stars](https://img.shields.io/github/stars/apache/arrow) | 列式数据格式 |

### 数据选择与过滤

| 框架 | Stars | 描述 |
|------|-------|------|
| [datamix](https://github.com/HelveticaErik/data-mix) | ![Stars](https://img.shields.io/github/stars/HelveticaErik/data-mix) | 高质量训练数据混合工具 |
| [Deduplicate](https://github.com/optimum-community/deduplicate) | ![Stars](https://img.shields.io/github/stars/optimum-community/deduplicate) | 数据去重工具 |

### 分词器

| 框架 | Stars | 描述 |
|------|-------|------|
| [tokenizers](https://github.com/huggingface/tokenizers) | ![Stars](https://img.shields.io/github/stars/huggingface/tokenizers) | 快速分词器 |
| [tiktoken](https://github.com/openai/tiktoken) | ![Stars](https://img.shields.io/github/stars/openai/tiktoken) | OpenAI 的快速分词器 |
| [sentencepiece](https://github.com/google/sentencepiece) | ![Stars](https://img.shields.io/github/stars/google/sentencepiece) | 无监督文本分词器 |

---

## 隐私与安全

### 本地与离线解决方案

| 框架 | Stars | 描述 |
|------|-------|------|
| [privateGPT](https://github.com/imartinez/privateGPT) | ![Stars](https://img.shields.io/github/stars/imartinez/privateGPT) | 离线私有 LLM 文档问答 |
| [GPT4All](https://github.com/nomic-ai/gpt4all) | ![Stars](https://img.shields.io/github/stars/nomic-ai/gpt4all) | 本地 LLM 聊天机器人生态系统 |
| [llamafile](https://github.com/Mozilla-Ocho/llamafile) | ![Stars](https://img.shields.io/github/stars/Mozilla-Ocho/llamafile) | 单文件可执行 LLM |
| [ollama](https://github.com/ollama/ollama) | ![Stars](https://img.shields.io/github/stars/ollama/ollama) | 本地运行 LLM |

### 开放隐私优先模型

| 框架 | Stars | 描述 |
|------|-------|------|
| [BLOOM](https://bigscience.github.io/bloom/) | - | 开源多语言大模型 |
| [Falcon](https://github.com/tiiuae/falcon-refinedweb) | ![Stars](https://img.shields.io/github/stars/tiiuae/falcon-refinedweb) | 阿联酋技术创新研究所的开源模型 |

---

## 垂直领域 LLM

### 医疗健康

| 框架 | Stars | 描述 |
|------|-------|------|
| [BioGPT](https://github.com/microsoft/BioGPT) | ![Stars](https://img.shields.io/github/stars/microsoft/BioGPT) | 生物医学领域 LLM |
| [Med-PaLM](https://sites.research.google/med-palm) | - | 医学领域大模型 |
| [Healthcare-LLM](https://github.com/WangRongsheng/HealthGPT) | ![Stars](https://img.shields.io/github/stars/WangRongsheng/HealthGPT) | 医疗健康领域 LLM |

### 代码与开发

| 框架 | Stars | 描述 |
|------|-------|------|
| [CodeLlama](https://github.com/meta-llama/codellama) | ![Stars](https://img.shields.io/github/stars/meta-llama/codellama) | 代码专用 LLaMA |
| [StarCoder](https://github.com/bigcodeproject/starcoder) | ![Stars](https://img.shields.io/github/stars/bigcodeproject/starcoder) | 代码生成大模型 |
| [CodeGen](https://github.com/salesforce/CodeGen) | ![Stars](https://img.shields.io/github/stars/salesforce/CodeGen) | Salesforce 的代码生成模型 |

### 金融

| 框架 | Stars | 描述 |
|------|-------|------|
| [BloombergGPT](https://bloomberg.com) | - | 彭博社金融领域 LLM |
| [FinGPT](https://github.com/ai4finance-foundation/fingpt) | ![Stars](https://img.shields.io/github/stars/ai4finance-foundation/fingpt) | 金融领域开源 LLM |

---

## RAG 与向量搜索

### RAG 框架

| 框架 | Stars | 描述 |
|------|-------|------|
| [LangChain](https://github.com/langchain-ai/langchain) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain) | LLM 应用框架 |
| [LlamaIndex](https://github.com/jerryjliu/llama_index) | ![Stars](https://img.shields.io/github/stars/jerryjliu/llama_index) | 数据增强 LLM 框架 |
| [RAGFlow](https://github.com/infiniflow/ragflow) | ![Stars](https://img.shields.io/github/stars/infiniflow/ragflow) | 基于深度文档理解的 RAG 引擎 |

### 向量数据库

| 框架 | Stars | 描述 |
|------|-------|------|
| [Milvus](https://github.com/milvus-io/milvus) | ![Stars](https://img.shields.io/github/stars/milvus-io/milvus) | 开源向量数据库 |
| [Qdrant](https://github.com/qdrant/qdrant) | ![Stars](https://img.shields.io/github/stars/qdrant/qdrant) | 向量相似度搜索引擎 |
| [Weaviate](https://github.com/weaviate/weaviate) | ![Stars](https://img.shields.io/github/stars/weaviate/weaviate) | 开源向量数据库 |
| [Chroma](https://github.com/chroma-core/chroma) | ![Stars](https://img.shields.io/github/stars/chroma-core/chroma) | AI 应用的向量数据库 |
| [pgvector](https://github.com/pgvector/pgvector) | ![Stars](https://img.shields.io/github/stars/pgvector/pgvector) | PostgreSQL 向量相似度搜索 |

---

## 评估与基准

### 评估框架

| 框架 | Stars | 描述 |
|------|-------|------|
| [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | ![Stars](https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness) | LLM 评估框架 |
| [promptfoo](https://github.com/promptfoo/promptfoo) | ![Stars](https://img.shields.io/github/stars/promptfoo/promptfoo) | 测试 prompts 和 LLM 输出 |
| [LangChain](https://github.com/langchain-ai/langchain) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain) | LLM 应用框架 |
| [ Inspect](https://github.com/UKGovernmentBEIS/inspect_ai) | ![Stars](https://img.shields.io/github/stars/UKGovernmentBEIS/inspect_ai) | LLM 评估框架 |

### 研究基准

| 基准 | 描述 |
|------|------|
| [MMLU](https://huggingface.co/datasets/cais/mmlu) | 多任务语言理解 |
| [HumanEval](https://github.com/openai/human-eval) | 代码生成评估 |
| [BBH](https://github.com/google-research/google-research/tree/master/bbh) | BIG-Bench Hard |
| [ARC](https://github.com/fchollet/ARC) | Abstraction and Reasoning Corpus |

---

## 科研工具

### 实验跟踪

| 框架 | Stars | 描述 |
|------|-------|------|
| [Weights & Biases](https://github.com/wandb/wandb) | ![Stars](https://img.shields.io/github/stars/wandb/wandb) | ML 实验跟踪 |
| [MLflow](https://github.com/mlflow/mlflow) | ![Stars](https://img.shields.io/github/stars/mlflow/mlflow) | ML 生命周期管理 |
| [TensorBoard](https://github.com/tensorflow/tensorboard) | ![Stars](https://img.shields.io/github/stars/tensorflow/tensorboard) | 可视化工具包 |
| [Aim](https://github.com/aimhubio/aim) | ![Stars](https://img.shields.io/github/stars/aimhubio/aim) | 自托管 ML 实验跟踪器 |

### 可视化与分析

| 框架 | Stars | 描述 |
|------|-------|------|
| [TransformerLens](https://github.com/TransformerLensOrg/TransformerLens) | ![Stars](https://img.shields.io/github/stars/TransformerLensOrg/TransformerLens) | Transformer 可视化与分析工具 |
| [PyVis](https://github.com/Westlake-AI/pygviz) | ![Stars](https://img.shields.io/github/stars/Westlake-AI/pygviz) | 神经网络可视化 |

---

## MLOps 与平台

### LLM 平台

| 框架 | Stars | 描述 |
|------|-------|------|
| [Ray](https://github.com/ray-project/ray) | ![Stars](https://img.shields.io/github/stars/ray-project/ray) | 分布式计算框架 |
| [SkyPilot](https://github.com/skypilot-org/skypilot) | ![Stars](https://img.shields.io/github/stars/skypilot-org/skypilot) | 多云 LLM 训练与推理 |
| [RunPod](https://github.com/runpod/runpod) | ![Stars](https://img.shields.io/github/stars/runpod/runpod) | GPU 云服务平台 |

---

## 部署与服务

### 模型服务平台

| 框架 | Stars | 描述 |
|------|-------|------|
| [Ray Serve](https://github.com/ray-project/ray) | ![Stars](https://img.shields.io/github/stars/ray-project/ray) | 可扩展模型服务 |
| [TorchServe](https://github.com/pytorch/serve) | ![Stars](https://img.shields.io/github/stars/pytorch/serve) | PyTorch 模型服务 |
| [Triton Inference Server](https://github.com/triton-inference-server/server) | ![Stars](https://img.shields.io/github/stars/triton-inference-server/server) | NVIDIA 推理服务器 |
| [BentoML](https://github.com/bentoml/BentoML) | ![Stars](https://img.shields.io/github/stars/bentoml/BentoML) | AI 应用统一平台 |
| [ONNX Runtime](https://github.com/microsoft/onnxruntime) | ![Stars](https://img.shields.io/github/stars/microsoft/onnxruntime) | 跨平台 ML 推理 |
| [OpenVINO](https://github.com/openvinotoolkit/openvino) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/openvino) | Intel 推理优化 |

---

## 监控与可观测性

### 训练监控

| 框架 | Stars | 描述 |
|------|-------|------|
| [Weights & Biases](https://github.com/wandb/wandb) | ![Stars](https://img.shields.io/github/stars/wandb/wandb) | ML 实验跟踪 |
| [MLflow](https://github.com/mlflow/mlflow) | ![Stars](https://img.shields.io/github/stars/mlflow/mlflow) | ML 生命周期管理 |
| [TensorBoard](https://github.com/tensorflow/tensorboard) | ![Stars](https://img.shields.io/github/stars/tensorflow/tensorboard) | 可视化工具包 |
| [Aim](https://github.com/aimhubio/aim) | ![Stars](https://img.shields.io/github/stars/aimhubio/aim) | 自托管 ML 实验跟踪器 |

### 推理监控

| 框架 | Stars | 描述 |
|------|-------|------|
| [LangSmith](https://github.com/langchain-ai/langsmith) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langsmith) | LLM 应用可观测性 |
| [LangFuse](https://github.com/langfuse/langfuse) | ![Stars](https://img.shields.io/github/stars/langfuse/langfuse) | 开源 LLM 工程平台 |
| [Phoenix](https://github.com/Arize-ai/phoenix) | ![Stars](https://img.shields.io/github/stars/Arize-ai/phoenix) | ML 可观测性平台 |
| [Helicone](https://github.com/Helicone/helicone) | ![Stars](https://img.shields.io/github/stars/Helicone/helicone) | 开源 LLM 可观测性 |

---

## 学习资源

### 官方文档

- [PyTorch 文档](https://pytorch.org/docs/) - 深度学习框架文档
- [Hugging Face 文档](https://huggingface.co/docs) - Transformers 和模型中心
- [DeepSpeed 文档](https://www.deepspeed.ai/getting-started/) - 分布式训练
- [vLLM 文档](https://docs.vllm.ai/) - 推理优化

### 教程与课程

- [DeepLearning.AI](https://www.deeplearning.ai/) - AI 课程
- [Fast.ai](https://www.fast.ai/) - 实践深度学习
- [Lightning Academy](https://lightning.ai/pages/education/) - ML 训练课程

---

## 贡献指南

欢迎贡献！请阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 了解指南。

## 许可证

[CC0 1.0 Universal](LICENSE) - 免费和开源。
