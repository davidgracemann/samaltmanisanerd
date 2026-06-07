# Graceman · Engineering Portfolio Scaffold
## Autonomous Systems & Adversarial AI — Recursive Learning Map

---

## Layer 0 — Language Foundation
*Everything else is built on these.*

```
Languages
├── Python          — primary research and AI engineering language
├── C++             — ROS2, HPC, embedded, performance-critical systems
├── CUDA C++        — GPU programming, kernel writing
├── Backend Engineering + System Design Fundmentals
└── Bash / Shell    — Linux internals, automation, deployment scripting
```

---

## Layer 1 — Scientific Computing

```
Scientific Stack
├── NumPy           — tensor operations, array computing
├── SciPy           — signal processing, optimization, linear algebra
├── JAX             — differentiable programming, hardware-accelerated research
├── Matplotlib      — visualization and analysis
└── Jupyter         — research experimentation environment
```

---

## Layer 2 — ML / AI Core

```
ML Frameworks
├── PyTorch                   — primary research framework
│   ├── torch.nn              — model construction
│   ├── torch.autograd        — automatic differentiation
│   ├── TorchScript           — model serialization
│   └── torch.distributed     — multi-GPU training
├── Hugging Face Transformers — model hub and transformer ecosystem
├── scikit-learn              — classical ML, evaluation pipelines
└── Weights & Biases          — experiment tracking
```

---

## Layer 3 — Domain Clusters

---

### [LLM] Applied AI Engineering
*The market-facing layer. Most hireable skillset right now regardless of research outcome.*

```
LLM Foundations
├── Model Ecosystem
│   ├── OpenAI API            — GPT-4o, o1, o3 family
│   ├── Anthropic API         — Claude family, tool use, MCP
│   ├── Gemini API            — Google multimodal family
│   ├── LiteLLM               — unified API across all providers
│   └── Hugging Face Hub      — open model access
│
├── Local LLM Stack
│   ├── Ollama                — local model serving (already using)
│   ├── vLLM                  — high-throughput production inference
│   ├── llama.cpp             — GGUF inference engine
│   ├── TGI                   — HuggingFace Text Generation Inference
│   └── LM Studio             — local model management
│
├── RAG (Retrieval Augmented Generation)
│   ├── Vector Databases
│   │   ├── ChromaDB          — local vector store (start here)
│   │   ├── Qdrant            — production-grade vector DB
│   │   ├── FAISS             — Facebook similarity search
│   │   └── Pinecone          — managed cloud vector DB
│   ├── Embedding Models
│   │   ├── text-embedding-3  — OpenAI embeddings
│   │   ├── BGE               — BAAI open embeddings
│   │   └── E5                — multilingual embeddings
│   ├── LlamaIndex            — RAG orchestration framework
│   └── RAGAS                 — RAG evaluation suite
│
├── Agentic Frameworks
│   ├── LangGraph             — stateful agent graphs (most important)
│   ├── LangChain             — legacy but widely used
│   ├── CrewAI                — multi-agent orchestration
│   ├── AutoGen               — Microsoft multi-agent framework
│   ├── OpenAI Agents SDK     — structured agent building
│   └── MCP                   — Model Context Protocol (Anthropic standard)
│
├── Fine-Tuning Stack
│   ├── LoRA / QLoRA          — parameter-efficient fine-tuning (PEFT)
│   ├── Unsloth               — fast fine-tuning (2x speed, less VRAM)
│   ├── Axolotl               — fine-tuning orchestration
│   ├── TRL                   — HuggingFace RLHF/DPO library
│   └── PEFT                  — HuggingFace PEFT library
│
├── Inference Optimization
│   ├── Flash Attention 2     — memory-efficient attention
│   ├── Speculative Decoding  — faster inference via draft models
│   ├── KV Cache              — key-value cache management
│   ├── GPTQ / AWQ            — weight quantization for LLMs
│   └── PagedAttention        — vLLM's memory management
│
├── Multimodal
│   ├── Vision-Language
│   │   ├── LLaVA             — open-source VLM
│   │   ├── Qwen-VL           — Alibaba VLM
│   │   ├── PaliGemma         — Google VLM
│   │   └── CLIP / SigLIP     — image-text embedding
│   ├── Speech
│   │   └── Whisper           — OpenAI speech recognition
│   └── Reasoning Models
│       ├── o1 / o3 style     — chain-of-thought reasoning architecture
│       └── DeepSeek-R1       — open reasoning model
│
├── Evaluation & Observability
│   ├── LangSmith             — LangChain tracing and evaluation
│   ├── Promptfoo             — prompt testing and CI
│   ├── OpenAI Evals          — evaluation framework
│   └── Arize Phoenix         — LLM observability
│
├── Production Deployment
│   ├── FastAPI               — LLM API serving
│   ├── Modal.com             — serverless GPU deployment
│   ├── RunPod                — GPU cloud for inference
│   ├── BentoML               — model packaging and serving
│   └── Streaming / SSE       — real-time token streaming
│
└── Trending Architecture Concepts (understand, not just use)
    ├── Mixture of Experts    — MoE routing and sparse activation
    ├── State Space Models    — Mamba, linear attention alternatives
    ├── Long Context Handling — RoPE scaling, YaRN, sliding window
    ├── Tool Use / Function Calling — structured LLM output
    ├── Computer Use Agents   — GUI and browser automation agents
    └── Prompt Injection & LLM Robustness — bridge to [AML] thesis
```

---

### [AML] Adversarial ML & Robustness
*Core of the research thesis.*

```
Adversarial ML
├── Attack Frameworks
│   ├── Foolbox           — model-agnostic adversarial attacks
│   ├── ART               — IBM Adversarial Robustness Toolbox
│   ├── Torchattacks      — PyTorch-native attack library
│   └── CleverHans        — reference attack implementations
├── Robustness Evaluation
│   ├── RobustBench       — standardised robustness benchmarking
│   └── AutoAttack        — reliable robustness evaluation protocol
├── OOD Detection
│   ├── PyOD              — outlier detection library
│   └── OpenOOD           — OOD benchmark suite
└── Neural Network Verification
    ├── Marabou           — DNN property verification
    ├── α,β-CROWN         — complete neural network verifier
    └── Z3                — SMT solver for formal property checking
```

---

### [CV] Computer Vision

```
Computer Vision
├── Core
│   ├── OpenCV            — image processing, classical CV
│   └── Pillow            — image I/O and preprocessing
├── Detection & Tracking
│   ├── Ultralytics YOLO  — object detection (v8, v11)
│   ├── MMDetection       — research-grade detection framework
│   ├── ByteTrack         — multi-object tracking
│   └── supervision       — detection pipeline utilities
├── Segmentation
│   ├── Segment Anything  — SAM (Meta)
│   └── Detectron2        — Facebook research framework
└── Datasets & Benchmarks
    └── COCO / Roboflow   — detection benchmarks and dataset tools
```

---

### [RAS] Robotics & Autonomous Systems

```
Robotics Stack
├── ROS2                  — Robot Operating System 2
│   ├── rclpy / rclcpp    — Python and C++ client libraries
│   ├── Nav2              — autonomous navigation
│   ├── MoveIt2           — motion planning
│   └── ros2_control      — hardware abstraction
├── Simulation
│   ├── Gazebo Harmonic   — physics simulation
│   ├── RViz2             — visualization
│   └── Webots            — alternative simulator
├── SLAM
│   ├── RTAB-Map          — RGB-D SLAM
│   ├── Cartographer      — Google SLAM
│   └── ORB-SLAM3         — visual SLAM
└── Path Planning
    ├── OMPL              — Open Motion Planning Library
    └── PythonRobotics    — reference algorithm implementations
```

---

### [EAI] Edge AI & Embedded Inference

```
Edge Inference
├── NVIDIA Stack
│   ├── TensorRT          — inference optimization
│   ├── TensorRT-LLM      — LLM inference on NVIDIA hardware
│   └── Jetson SDK        — edge deployment
├── Cross-Platform
│   ├── ONNX Runtime      — cross-platform inference
│   └── OpenVINO          — Intel optimization
└── Quantization
    ├── PyTorch Quantization — INT8/FP16
    ├── GPTQ / AWQ        — LLM quantization
    └── llama.cpp         — GGUF inference
```

---

### [SE] Systems Engineering

```
Systems Stack
├── Docker / Podman       — containerization
├── Kubernetes / K3s      — orchestration
├── Terraform / Ansible   — infrastructure as code
├── Prometheus / Grafana  — monitoring
└── Networking
    ├── Wireshark         — packet analysis
    └── iperf3            — performance testing
```

---

### [SPW] Signal Processing & EW

```
Signal Processing
├── SciPy.signal          — filtering, FFT, spectral analysis
├── PyWavelets            — wavelet transforms
├── GNU Radio             — SDR framework
├── PySDR                 — SDR in Python
└── RTL-SDR               — hardware entry point
```

---

### [HWE] Hardware & Embedded

```
Hardware Stack
├── FPGA
│   ├── Xilinx Vivado     — synthesis and implementation
│   ├── Vitis HLS         — high-level synthesis
│   └── VHDL / Verilog    — HDL languages
├── MCU
│   ├── STM32 (HAL/LL)    — primary target
│   └── PlatformIO        — embedded development environment
└── FreeRTOS              — real-time operating system
```

---

### [HPC] High Performance Computing

```
HPC Stack
├── CUDA C++              — kernel writing
├── cuBLAS / cuDNN        — GPU primitives
├── Triton                — OpenAI GPU language
├── CuPy                  — NumPy on GPU
└── Nsight Systems        — GPU profiling
```

---

## Layer 4 — Formal Methods

```
Formal Methods
├── TLA+                  — temporal logic specification
├── Z3                    — SMT solver (most practical entry)
├── SPIN                  — model checking
├── Marabou               — neural network verification
└── Coq                   — proof assistant (long-game)
```

---

## Layer 5 — Research Infrastructure

```
│
├── Inference Optimization
│   ├── Flash Attention 2     — memory-efficient attention
│   ├── Speculative Decoding  — faster inference via draft models
│   ├── KV Cache              — key-value cache management
│   ├── GPTQ / AWQ            — weight quantization for LLMs
│   └── PagedAttention        — vLLM's memory management
│
├── Multimodal
Research Stack
├── LaTeX                 — paper writing
├── Git + DVC             — version and data control
├── CMake                 — C++ build system
├── uv                    — Python packaging (already using)
├── MLflow / W&B          — experiment management
└── arXiv / Papers With Code — research discovery
```

---

## Recursive Dependency Map

```
[LLM]  ─── needs ──→ Layer 0 (Python), Layer 2 (HuggingFace)
[AML]  ─── needs ──→ Layer 0, 1, 2, [LLM] (for LLM robustness angle)
[CV]   ─── needs ──→ Layer 0, 1, 2
[RAS]  ─── needs ──→ Layer 0, [CV]
[EAI]  ─── needs ──→ Layer 0, 2, [CV], [LLM] (TensorRT-LLM)
[SE]   ─── needs ──→ Layer 0 (Bash)
[SPW]  ─── needs ──→ Layer 0, 1
[HWE]  ─── needs ──→ C++, Layer 0
[HPC]  ─── needs ──→ CUDA C++, Layer 0
Formal ─── needs ──→ Layer 0, [AML]
```

---

## What To Actually Build Right Now (Semester 1)

```
Active this semester
├── PyTorch               — Layer 2 foundation, everything sits on this
├── [LLM] core            — API usage, RAG basics, LangGraph (most hireable now)
├── [AML] basics          — Foolbox + ART (thesis direction)
└── CUDA basics           — RTX 5070 sitting idle otherwise
```

*The rest of the scaffold is the 2-year reference map. Pull from it as projects demand.*

---

*Graceman Skill Scaffold · June 2026*
