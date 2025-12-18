
# Embedl

Embedl develops advanced tools and algorithms for **Edge AI**. Our mission is to make AI models run 
**faster**, **more energy-efficient**, and **reliably across diverse hardware platforms**, while 
significantly reducing development time.

We help teams deploy high-performance AI on real-world, resource-constrained devices.

---

## Core Products

### **Embedl SDK** *[Enterprise](https://www.embedl.com/sdk)*

A **source-available**, toolkit that supports the **entire Edge AI development lifecycle**.  
The SDK integrates with **any hardware or toolchain**, including:

- NVIDIA GPUs (Jetson AGX Orin, Nano, Thor, Drive Thor … )
- Qualcomm & TI accelerators 
- CPUs, MCUs, FPGAs, and custom accelerators  

The SDK follows Embedl’s **C3PO Framework**:

- **Compatibility** – through model surgery to fix op support issues 
- **Provisioning** – of hardware access, runtimes, and compilation servers 
- **Pipeline** – to compile, quantize, and run on-device inference for any model and hardware  
- **Profiling** – on-device latency, memory, and performance for layerwise statistics  
- **Optimization** – with public and proprietary algorithms for:
  - Mixed-precision quantization  
  - Pruning
  - Neural Architecture Search (NAS)
  - Knowledge Distillation  

---

### **Embedl Hub** *[Free Beta](https://hub.embedl.com)*  

A cloud-based platform for **quantization, compilation, benchmarking, and deployment** on real edge
devices (Android & iOS) through device farms.

Key features:

- Run models on real devices via the cloud  
- Profile latency and performance  
- Track experiments and compare results across devices  
- Deploy optimized models directly to edge environments  

---

### **Embedl Visualizer** *(Enterprise)*
A powerful visualization tool for understanding model performance across the stack.

Supports:
- PyTorch & ONNX models  
- Compiled artifacts (TensorRT engines, TIDL graphs, etc.)

Capabilities:
- Identify latency bottlenecks quickly  
- Debug QAT issues caused by operator fusion  
- Compare multiple models and configurations  
- Track how a model evolves across compilation stages — from Python code to final deployable binaries  

---

### **Embedl Models** ([Community](https://huggingface.co/embedl))

Pre-optimized models that can be used **off-the-shelf** or customized for specific hardware target
supported by the [embedl-models](https://github.com/embedl/embedl-models) package.

**First release highlights:**

- The **fastest Small Language Models (SLMs)** using **[FlashHead](https://www.embedl.com/knowledge/ultra-efficient-llms-embedls-breakthrough-for-on-device-ai)**,
  a novel architectural improvement to the language-model head
- Works with popular models like **Llama, Gemma, and Qwen**
- Provides speedups on top of:
  - Quantization  
  - Flash Attention  
  - Other standard optimizations
  - 

| Device: Nvidia Jetson Thor                       |                             |
| Model                                            | Generation speed (tokens/s) |
| ------------------------------------------------ | ----------------------------|
| embedl/Llama-3.2-3B-Instruct-FlashHead-W4A16     | 100                         |
| Llama-3.2-3B-Instruct-W4A16*                     | 80                          |
| RedHatAI/Llama-3.2-3B-Instruct-FP8               | 64                          |
| meta-llama/Llama-3.2-3B-Instruct                 | 37                          |

*Embedl quantized model for benchmarking similar to the FlashHead-W4A16 but without
the faster FlashHead and custom generation loop.

---

## Why It Matters

- Enables AI deployment on **resource-constrained hardware**:
  - Embedded systems  
  - Mobile devices  
  - IoT  
  - Robotics  
- Reduces **latency, memory usage, and energy consumption**, enabling real-time inference without 
  cloud dependence  
- Saves development time through a **hardware-agnostic workflow** reusable across models and platforms  
- Bridges the gap between **academic ML research** and **industrial embedded AI applications**

---

## Company Information

- **Founded:** 2018 (spin-out from Chalmers University of Technology)  
- **Commercial Operations:** Since 2022  
- **Headquarters:** Gothenburg, Sweden  
- **US Office:** Palo Alto, California  
- **Recognition:**  
  - Named to **CB Insights “AI 100” (2025)** list of the most promising private AI companies  

---

## Typical Use Cases

Embedl is used where **real-time performance and efficiency are critical**:

- **Automotive & Autonomous Systems**
  - Autonomous driving
  - ADAS
  - Driver monitoring
  - Predictive maintenance  
  - *Example: Kodiak Robotics*

- **Defense & Aerospace**
  - Secure, energy-constrained AI inference  
  - *Example: Airbus*

- **Mobile & Edge AI**
  - Running deep-learning models directly on phones and embedded devices  
  - No cloud dependency via Embedl Hub  

---

## How to Get Started

### **Quick Start with Embedl Hub**
- Upload your model (PyTorch or ONNX)  
- Quantize, compile, and benchmark on supported devices  
- No physical hardware required  

### **Full Control with Embedl SDK**
- Integrate Embedl directly into your training and deployment pipeline  
- Works with TensorRT, QNN, TIDL, and more  
- Access advanced hardware-aware optimization and performance insights  
- Deploy to your own infrastructure  

### **Custom & Enterprise Needs**
For tailored optimizations, specialized hardware support, and engineering collaboration, contact 
Embedl for full SDK access and support.

---

## Contact

**Headquarters (Sweden)**  
Gamla Almedalsvägen 39  
412 63 Gothenburg, Sweden  

📧 **Email:** info@embedl.com

