# Awesome LLM Training & Inference

> Curated list of frameworks, tools, and resources for LLM training and inference. Covers the full pipeline from data processing to deployment.

[![License](https://img.shields.io/badge/license-CC0--1.0-blue)](LICENSE)

<!-- keywords: LLM, large language model, training, inference, deep learning, machine learning, PyTorch, transformers, distributed training, model serving -->

## Contents

- [Training Frameworks](#training-frameworks)
- [Pretraining Implementations](#pretraining-implementations)
- [End-to-End Training & Inference](#end-to-end-training--inference)
- [Inference Frameworks](#inference-frameworks)
- [Distributed Training](#distributed-training)
- [Hardware Acceleration](#hardware-acceleration)
- [Fine-Tuning & PEFT](#fine-tuning--peft)
- [Model Compression & Quantization](#model-compression--quantization)
- [Data Engineering](#data-engineering)
- [Privacy & Security](#privacy--security)
- [Domain-Specific LLMs](#domain-specific-llms)
- [RAG & Vector Search](#rag--vector-search)
- [Evaluation & Benchmarking](#evaluation--benchmarking)
- [Research Tools](#research-tools)
- [MLOps & Platform](#mlops--platform)
- [Deployment & Serving](#deployment--serving)
- [Monitoring & Observability](#monitoring--observability)
- [Learning Resources](#learning-resources)
- [Contributing](#contributing)
- [License](#license)

---

## Training Frameworks

### Deep Learning Frameworks

| Framework | Stars | Description |
|-----------|-------|-------------|
| [PyTorch](https://github.com/pytorch/pytorch) | ![Stars](https://img.shields.io/github/stars/pytorch/pytorch) | Open source machine learning framework |
| [transformers](https://github.com/huggingface/transformers) | ![Stars](https://img.shields.io/github/stars/huggingface/transformers) | State-of-the-art ML for text, vision, audio |
| [JAX](https://github.com/google/jax) | ![Stars](https://img.shields.io/github/stars/google/jax) | Composable transformations for ML |
| [Flax](https://github.com/google/flax) | ![Stars](https://img.shields.io/github/stars/google/flax) | Neural network library for JAX |

### Training Libraries

| Framework | Stars | Description |
|-----------|-------|-------------|
| [Accelerate](https://github.com/huggingface/accelerate) | ![Stars](https://img.shields.io/github/stars/huggingface/accelerate) | Easy distributed training in PyTorch |
| [Lightning](https://github.com/Lightning-AI/pytorch-lightning) | ![Stars](https://img.shields.io/github/stars/Lightning-AI/pytorch-lightning) | Deep learning framework for scalable training |
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/deepspeedai/DeepSpeed) | Deep learning optimization and RLHF training |
| [Fairscale](https://github.com/facebookresearch/fairscale) | ![Stars](https://img.shields.io/github/stars/facebookresearch/fairscale) | PyTorch extensions for high-performance training |
| [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | ![Stars](https://img.shields.io/github/stars/NVIDIA/Megatron-LM) | Large-scale transformer training |
| [ColossalAI](https://github.com/hpcaitech/ColossalAI) | ![Stars](https://img.shields.io/github/stars/hpcaitech/ColossalAI) | Large-scale model training system |

---

## Pretraining Implementations

### From-Scratch Implementations

| Framework | Stars | Description |
|-----------|-------|-------------|
| [nanoGPT](https://github.com/karpathy/nanoGPT) | ![Stars](https://img.shields.io/github/stars/karpathy/nanoGPT) | Minimal GPT-2 training implementation by Karpathy |
| [lit-llama](https://github.com/Lightning-AI/lit-llama) | ![Stars](https://img.shields.io/github/stars/Lightning-AI/lit-llama) | LLaMA implementation based on nanoGPT, Apache 2.0 licensed |
| [GPT-NeoX](https://github.com/EleutherAI/gpt-neox) | ![Stars](https://img.shields.io/github/stars/EleutherAI/gpt-neox) | Large-scale autoregressive transformers by EleutherAI |
| [lunariscodex](https://github.com/MeryylleA/lunariscodex) | ![Stars](https://img.shields.io/github/stars/MeryylleA/lunariscodex) | High-performance Llama-style pre-training toolkit |

###RWKV

| Framework | Stars | Description |
|-----------|-------|-------------|
| [nanoRWKV](https://github.com/Hannibal046/nanoRWKV) | ![Stars](https://img.shields.io/github/stars/Hannibal046/nanoRWKV) | nanoGPT-style RWKV implementation - RNN with GPT-level performance |

---

## End-to-End Training & Inference

### End-to-End Fine-Tuning

| Framework | Stars | Description |
|-----------|-------|-------------|
| [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) | ![Stars](https://img.shields.io/github/stars/axolotl-ai-cloud/axolotl) | YAML-driven LLM fine-tuning toolkit |
| [LlamaFactory](https://github.com/hiyouga/LlamaFactory) | ![Stars](https://img.shields.io/github/stars/hiyouga/LlamaFactory) | Unified efficient fine-tuning of 100+ LLMs |
| [TRL](https://github.com/huggingface/trl) | ![Stars](https://img.shields.io/github/stars/huggingface/trl) | Train language models with RLHF and DPO |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/microsoft/DeepSpeed) | Easy-to-use RLHF training pipeline |

### End-to-End Inference

| Framework | Stars | Description |
|-----------|-------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm) | High-throughput LLM inference engine |
| [Ollama](https://github.com/ollama/ollama) | ![Stars](https://img.shields.io/github/stars/ollama/ollama) | Run LLMs locally |
| [SGLang](https://github.com/sgl-project/sglang) | ![Stars](https://img.shields.io/github/stars/sgl-project/sglang) | High-performance serving framework for LLMs |
| [Text Generation Inference](https://github.com/huggingface/text-generation-inference) | ![Stars](https://img.shields.io/github/stars/huggingface/text-generation-inference) | Hugging Face's production-ready inference server |

---

## Inference Frameworks

### High-Performance Inference

| Framework | Stars | Description |
|-----------|-------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm) | High-throughput LLM inference engine |
| [SGLang](https://github.com/sgl-project/sglang) | ![Stars](https://img.shields.io/github/stars/sgl-project/sglang) | High-performance serving framework for LLMs |
| [Text Generation Inference](https://github.com/huggingface/text-generation-inference) | ![Stars](https://img.shields.io/github/stars/huggingface/text-generation-inference) | Hugging Face's production-ready inference server |
| [LightLLM](https://github.com/ModelTC/LightLLM) | ![Stars](https://img.shields.io/github/stars/ModelTC/LightLLM) | Lightweight LLM inference framework |
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | ![Stars](https://img.shields.io/github/stars/ggerganov/llama.cpp) | LLM inference in C/C++ |
| [Ollama](https://github.com/ollama/ollama) | ![Stars](https://img.shields.io/github/stars/ollama/ollama) | Run LLMs locally |
| [ktransformers](https://github.com/kvcache-ai/ktransformers) | ![Stars](https://img.shields.io/github/stars/kvcache-ai/ktransformers) | Flexible framework for heterogeneous LLM inference optimizations |
| [GPUSstack](https://github.com/gpustack/gpustack) | ![Stars](https://img.shields.io/github/stars/gpustack/gpustack) | Performance-optimized AI inference on GPUs |
| [JetStream](https://github.com/AI-Hypercomputer/JetStream) | ![Stars](https://img.shields.io/github/stars/AI-Hypercomputer/JetStream) | Throughput-optimized engine for LLM inference on XLA devices |
| [NanoLLM](https://github.com/dusty-nv/NanoLLM) | ![Stars](https://img.shields.io/github/stars/dusty-nv/NanoLLM) | Optimized local inference with quantization and vision models |

### Local & Edge Inference

| Framework | Stars | Description |
|-----------|-------|-------------|
| [LM Studio](https://github.com/lmstudio-ai/lmstudio) | ![Stars](https://img.shields.io/github/stars/lmstudio-ai/lmstudio) | Discover and run local LLMs |
| [IPEX-LLM](https://github.com/intel/ipex-llm) | ![Stars](https://img.shields.io/github/stars/intel/ipex-llm) | Accelerate LLM inference on Intel hardware |
| [vLLM-MLX](https://github.com/waybarrios/vllm-mlx) | ![Stars](https://img.shields.io/github/stars/waybarrios/vllm-mlx) | OpenAI-compatible LLM server for Apple Silicon |
| [o/mlx](https://github.com/jundot/omlx) | ![Stars](https://img.shields.io/github/stars/jundot/omlx) | LLM inference server with continuous batching for Apple Silicon |

### Multi-LoRA Serving

| Framework | Stars | Description |
|-----------|-------|-------------|
| [LoRAX](https://github.com/predibase/lorax) | ![Stars](https://img.shields.io/github/stars/predibase/lorax) | Multi-LoRA inference server that scales to 1000s of fine-tuned LLMs |

---

## Distributed Training

### Parallel Training Frameworks

| Framework | Stars | Description |
|-----------|-------|-------------|
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/deepspeedai/DeepSpeed) | Distributed training with ZeRO optimization |
| [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | ![Stars](https://img.shields.io/github/stars/NVIDIA/Megatron-LM) | Large-scale transformer training |
| [ColossalAI](https://github.com/hpcaitech/ColossalAI) | ![Stars](https://img.shields.io/github/stars/hpcaitech/ColossalAI) | Large-scale model training system |

### Training Optimizations

| Framework | Stars | Description |
|-----------|-------|-------------|
| [FlashAttention](https://github.com/Dao-AILab/flash-attention) | ![Stars](https://img.shields.io/github/stars/Dao-AILab/flash-attention) | Fast and memory-efficient attention |
| [xFormers](https://github.com/facebookresearch/xformers) | ![Stars](https://img.shields.io/github/stars/facebookresearch/xformers) | Modular components for transformers |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/microsoft/DeepSpeed) | Easy-to-use RLHF training pipeline |

### Hardware Acceleration

| Framework | Stars | Description |
|-----------|-------|-------------|
| [IPEX-LLM](https://github.com/intel/ipex-llm) | ![Stars](https://img.shields.io/github/stars/intel/ipex-llm) | LLM inference acceleration on Intel GPUs/CPU |
| [OpenVINO](https://github.com/openvinotoolkit/openvino) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/openvino) | Intel hardware inference optimization toolkit |
| [Triton](https://github.com/triton-inference-server/triton) | ![Stars](https://img.shields.io/github/stars/triton-inference-server/triton) | Open-source GPU inference server |

---

## Fine-Tuning & PEFT

### Parameter-Efficient Fine-Tuning

| Framework | Stars | Description |
|-----------|-------|-------------|
| [PEFT](https://github.com/huggingface/peft) | ![Stars](https://img.shields.io/github/stars/huggingface/peft) | State-of-the-art parameter-efficient fine-tuning |
| [LlamaFactory](https://github.com/hiyouga/LlamaFactory) | ![Stars](https://img.shields.io/github/stars/hiyouga/LlamaFactory) | Unified efficient fine-tuning of 100+ LLMs |
| [xTuring](https://github.com/stochasticai/xTuring) | ![Stars](https://img.shields.io/github/stars/stochasticai/xTuring) | Build, personalize and control your own LLMs |
| [Unsloth](https://github.com/unslothai/unsloth) | ![Stars](https://img.shields.io/github/stars/unslothai/unsloth) | Memory-efficient fine-tuning (2x faster, 70% less memory) |
| [ArcticTraining](https://github.com/snowflakedb/ArcticTraining) | ![Stars](https://img.shields.io/github/stars/snowflakedb/ArcticTraining) | Snowflake's LLM post-training framework |
| [SteptronOss](https://github.com/stepfun-ai/SteptronOss) | ![Stars](https://img.shields.io/github/stars/stepfun-ai/SteptronOss) | Lightweight AI-native training framework for LLMs |

### RLHF & Alignment

| Framework | Stars | Description |
|-----------|-------|-------------|
| [TRL](https://github.com/huggingface/trl) | ![Stars](https://img.shields.io/github/stars/huggingface/trl) | Train language models with RLHF and DPO |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeed) | ![Stars](https://img.shields.io/github/stars/microsoft/DeepSpeed) | Easy-to-use RLHF training pipeline |

---

## Model Compression & Quantization

### Quantization Tools

| Framework | Stars | Description |
|-----------|-------|-------------|
| [BitsAndBytes](https://github.com/TimDettmers/bitsandbytes) | ![Stars](https://img.shields.io/github/stars/TimDettmers/bitsandbytes) | 8-bit quantization for LLMs |
| [AWQ](https://github.com/mit-han-lab/awq) | ![Stars](https://img.shields.io/github/stars/mit-han-lab/awq) | Activation-aware weight quantization |
| [GPTQ](https://github.com/IST-DASLab/gptq) | ![Stars](https://img.shields.io/github/stars/IST-DASLab/gptq) | GPT post-training quantization |
| [GGML](https://github.com/ggerganov/ggml) | ![Stars](https://img.shields.io/github/stars/ggerganov/ggml) | Tensor library for ML |
| [exllamav2](https://github.com/turboderp-org/exllamav2) | ![Stars](https://img.shields.io/github/stars/turboderp-org/exllamav2) | Optimized quantization for running LLMs on consumer GPUs |

### Compression Frameworks

| Framework | Stars | Description |
|-----------|-------|-------------|
| [NNCF](https://github.com/openvinotoolkit/nncf) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/nncf) | Neural network compression framework |
| [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | ![Stars](https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM) | NVIDIA's LLM inference optimization |
| [Optimum](https://github.com/huggingface/optimum) | ![Stars](https://img.shields.io/github/stars/huggingface/optimum) | Optimization tools for transformers |
| [Model-Optimizer](https://github.com/NVIDIA/Model-Optimizer) | ![Stars](https://img.shields.io/github/stars/NVIDIA/Model-Optimizer) | Unified SOTA model optimization techniques (quantization, pruning, distillation) |

---

## Data Engineering

### Data Processing

| Framework | Stars | Description |
|-----------|-------|-------------|
| [DataLoader](https://github.com/pytorch/data) | ![Stars](https://img.shields.io/github/stars/pytorch/data) | Data loading utility for PyTorch |
| [Datasets](https://github.com/huggingface/datasets) | ![Stars](https://img.shields.io/github/stars/huggingface/datasets) | Public datasets for ML |
| [WebDataset](https://github.com/webdataset/webdataset) | ![Stars](https://img.shields.io/github/stars/webdataset/webdataset) | Large-scale dataset handling |
| [PyArrow](https://github.com/apache/arrow) | ![Stars](https://img.shields.io/github/stars/apache/arrow) | Columnar data format |

### Data Selection & Filtering

| Framework | Stars | Description |
|-----------|-------|-------------|
| [DSIR](https://github.com/p-lambda/dsir) | ![Stars](https://img.shields.io/github/stars/p-lambda/dsir) | Large-scale data selection for language model training |

### Tokenizers

| Framework | Stars | Description |
|-----------|-------|-------------|
| [tiktoken](https://github.com/openai/tiktoken) | ![Stars](https://img.shields.io/github/stars/openai/tiktoken) | Fast BPE tokenizer by OpenAI |
| [sentencepiece](https://github.com/google/sentencepiece) | ![Stars](https://img.shields.io/github/stars/google/sentencepiece) | Unsupervised text tokenizer |

---

## Privacy & Security

### Local & Offline Solutions

| Framework | Stars | Description |
|-----------|-------|-------------|
| [privateGPT](https://github.com/imartinez/privateGPT) | ![Stars](https://img.shields.io/github/stars/imartinez/privateGPT) | Private Q&A with local LLMs, 100% offline |
| [GPT4All](https://github.com/nomic-ai/gpt4all) | ![Stars](https://img.shields.io/github/stars/nomic-ai/gpt4all) | Open-source LLM ecosystem you can run anywhere |
| [llamafile](https://github.com/Mozilla-OA/llamafile) | ![Stars](https://img.shields.io/github/stars/Mozilla-OA/llamafile) | Single-file LLM distribution |

### Open Privacy-Focused Models

| Model | Description |
|-------|-------------|
| [BLOOM](https://bigscience.huggingface.org/bloom) | BigScience open-access multilingual model |
| [Falcon](https://falconllm.tii.ae/) | Technology Innovation Institute's open models |

---

## Domain-Specific LLMs

### Healthcare & Medical

| Framework | Stars | Description |
|-----------|-------|-------------|
| [BioGPT](https://github.com/microsoft/BioGPT) | ![Stars](https://img.shields.io/github/stars/microsoft/BioGPT) | Biomedical language model by Microsoft |
| [Med-PaLM](https://github.com/Stanford-AI-Lab/Med-PaLM) | ![Stars](https://img.shields.io/github/stars/Stanford-AI-Lab/Med-PaLM) | Medical domain LLM by Stanford |
| [Healthcare-LLM](https://github.com/kangjiayin/Healthcare-LLM) | ![Stars](https://img.shields.io/github/stars/kangjiayin/Healthcare-LLM) | Healthcare-specific fine-tuning |

### Code & Development

| Framework | Stars | Description |
|-----------|-------|-------------|
| [CodeLlama](https://github.com/facebookresearch/codellama) | ![Stars](https://img.shields.io/github/stars/facebookresearch/codellama) | Code-specialized Llama by Meta |
| [StarCoder](https://github.com/bigcode-project/starcoder) | ![Stars](https://img.shields.io/github/stars/bigcode-project/starcoder) | Open code generation model by BigCode |
| [CodeGen](https://github.com/salesforce/CodeGen) | ![Stars](https://img.shields.io/github/stars/salesforce/CodeGen) | Open code generation models |

### Finance

| Framework | Description |
|-----------|-------------|
| [BloombergGPT](https://bloomberg.com/company/press/bloomberg-gpt-50-billion-parameter-llm-purpose-built-finance) | Financial domain LLM |
| [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | Open-source financial LLM |

---

## RAG & Vector Search

### RAG Frameworks

| Framework | Stars | Description |
|-----------|-------|-------------|
| [AutoRAG](https://github.com/Marker-Inc-Korea/AutoRAG) | ![Stars](https://img.shields.io/github/stars/Marker-Inc-Korea/AutoRAG) | Open-Source RAG evaluation & optimization framework |
| [RAGLAB](https://github.com/fate-ubw/RAGLAB) | ![Stars](https://img.shields.io/github/stars/fate-ubw/RAGLAB) | Modular research-oriented RAG framework |
| [cognita](https://github.com/truefoundry/cognita) | ![Stars](https://img.shields.io/github/stars/truefoundry/cognita) | Modular RAG framework for production |
| [canopy](https://github.com/pinecone-io/canopy) | ![Stars](https://img.shields.io/github/stars/pinecone-io/canopy) | RAG framework powered by Pinecone |

### Vector Databases

| Framework | Stars | Description |
|-----------|-------|-------------|
| [Milvus](https://github.com/milvus-io/milvus) | ![Stars](https://img.shields.io/github/stars/milvus-io/milvus) | Open-source vector database for AI |
| [Qdrant](https://github.com/qdrant/qdrant) | ![Stars](https://img.shields.io/github/stars/qdrant/qdrant) | Vector similarity search engine |
| [Weaviate](https://github.com/weaviate/weaviate) | ![Stars](https://img.shields.io/github/stars/weaviate/weaviate) | Open source vector database |
| [Chroma](https://github.com/chroma-core/chroma) | ![Stars](https://img.shields.io/github/stars/chroma-core/chroma) | AI-native embeddings database |
| [Infinity](https://github.com/infiniflow/infinity) | ![Stars](https://img.shields.io/github/stars/infiniflow/infinity) | AI-native database for LLM applications |
| [Kuzu](https://github.com/kuzudb/kuzu) | ![Stars](https://img.shields.io/github/stars/kuzudb/kuzu) | Embedded graph DB with vector search |
| [sqlite-vector](https://github.com/sqliteai/sqlite-vector) | ![Stars](https://img.shields.io/github/stars/sqliteai/sqlite-vector) | SQLite vector search extension |

---

## Evaluation & Benchmarking

### Evaluation Frameworks

| Framework | Stars | Description |
|-----------|-------|-------------|
| [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | ![Stars](https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness) | LLM evaluation framework |
| [promptfoo](https://github.com/promptfoo/promptfoo) | ![Stars](https://img.shields.io/github/stars/promptfoo/promptfoo) | Test prompts and LLM outputs |
| [LangChain](https://github.com/langchain-ai/langchain) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain) | LLM application framework |
| [Awesome-LLM-Eval](https://github.com/onejune2018/Awesome-LLM-Eval) | ![Stars](https://img.shields.io/github/stars/onejune2018/Awesome-LLM-Eval) | Curated list of LLM evaluation tools and benchmarks |

### Research Benchmarks

| Benchmark | Description |
|-----------|-------------|
| [MMLU](https://huggingface.co/datasets/llm-benchmarks/MMLU) | Multi-task language understanding |
| [HumanEval](https://github.com/openai/human-eval) | Code generation evaluation |
| [BBH](https://github.com/google-research/google-research/tree/master/big_bench) | Big Bench Hard - challenging tasks |
| [IFEval](https://github.com/google-research/google-research/tree/master/if_eval) | Instruction following evaluation |

---

## Research Tools

### Experiment Tracking

| Framework | Stars | Description |
|-----------|-------|-------------|
| [Weights & Biases](https://github.com/wandb/wandb) | ![Stars](https://img.shields.io/github/stars/wandb/wandb) | ML experiment tracking |
| [MLflow](https://github.com/mlflow/mlflow) | ![Stars](https://img.shields.io/github/stars/mlflow/mlflow) | ML lifecycle management |
| [TensorBoard](https://github.com/tensorflow/tensorboard) | ![Stars](https://img.shields.io/github/stars/tensorflow/tensorboard) | Visualization toolkit |
| [Aim](https://github.com/aimhubio/aim) | ![Stars](https://img.shields.io/github/stars/aimhubio/aim) | Self-hosted ML experiment tracker |

### Visualization & Analysis

| Framework | Stars | Description |
|-----------|-------|-------------|
| [TransformerLens](https://github.com/TransformerLensOrg/TransformerLens) | ![Stars](https://img.shields.io/github/stars/TransformerLensOrg/TransformerLens) | Interpretability for GPT-style models |
| [PyVis](https://github.com/Han-Lee/PyVis) | ![Stars](https://img.shields.io/github/stars/Han-Lee/PyVis) | Neural network visualization |

---

## MLOps & Platform

### LLM Platforms

| Framework | Stars | Description |
|-----------|-------|-------------|
| [StarWhale](https://github.com/star-whale/starwhale) | ![Stars](https://img.shields.io/github/stars/star-whale/starwhale) | MLOps/LLMOps platform |
| [Flyte](https://github.com/flyteorg/flyte) | ![Stars](https://img.shields.io/github/stars/flyteorg/flyte) | Scalable workflow orchestration platform |
| [Ray](https://github.com/ray-project/ray) | ![Stars](https://img.shields.io/github/stars/ray-project/ray) | Distributed computing for AI |

---

## Deployment & Serving

### Model Serving Platforms

| Framework | Stars | Description |
|-----------|-------|-------------|
| [Ray Serve](https://github.com/ray-project/ray) | ![Stars](https://img.shields.io/github/stars/ray-project/ray) | Scalable model serving |
| [TorchServe](https://github.com/pytorch/serve) | ![Stars](https://img.shields.io/github/stars/pytorch/serve) | PyTorch model serving |
| [Triton Inference Server](https://github.com/triton-inference-server/server) | ![Stars](https://img.shields.io/github/stars/triton-inference-server/server) | NVIDIA's inference server |
| [BentoML](https://github.com/bentoml/BentoML) | ![Stars](https://img.shields.io/github/stars/bentoml/BentoML) | Unified platform for AI apps |
| [ONNX Runtime](https://github.com/microsoft/onnxruntime) | ![Stars](https://img.shields.io/github/stars/microsoft/onnxruntime) | Cross-platform ML inference |
| [OpenVINO](https://github.com/openvinotoolkit/openvino) | ![Stars](https://img.shields.io/github/stars/openvinotoolkit/openvino) | Intel's inference optimization |

---

## Monitoring & Observability

| Framework | Stars | Description |
|-----------|-------|-------------|
| [LangSmith](https://github.com/langchain-ai/langsmith) | ![Stars](https://img.shields.io/github/stars/langchain-ai/langsmith) | LLM application observability |
| [LangFuse](https://github.com/langfuse/langfuse) | ![Stars](https://img.shields.io/github/stars/langfuse/langfuse) | Open-source LLM engineering platform |
| [Phoenix](https://github.com/Arize-ai/phoenix) | ![Stars](https://img.shields.io/github/stars/Arize-ai/phoenix) | ML observability platform |
| [Helicone](https://github.com/Helicone/helicone) | ![Stars](https://img.shields.io/github/stars/Helicone/helicone) | Open-source LLM observability |

---

## Learning Resources

### Official Documentation

- [PyTorch Documentation](https://pytorch.org/docs/) - Deep learning framework docs
- [Hugging Face Docs](https://huggingface.co/docs) - Transformers and model hub
- [DeepSpeed Documentation](https://www.deepspeed.ai/getting-started/) - Distributed training
- [vLLM Documentation](https://docs.vllm.ai/) - Inference optimization

### Tutorials & Courses

- [DeepLearning.AI](https://www.deeplearning.ai/) - AI courses
- [Fast.ai](https://www.fast.ai/) - Practical deep learning
- [Lightning Academy](https://lightning.ai/pages/education/) - ML training courses

---

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License

[CC0 1.0 Universal](LICENSE) - Free and open source.
