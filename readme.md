# 端到端语音交互系统

## 任务
- **ASR (自动语音识别)**：将语音转化为文本。
- **S2TT (语音到文本翻译)**：语音翻译为文本。
- **SER (语音情感识别)**：识别语音中的情感。
- **VSC (语音风格转换)**：改变语音的风格。
- **AIR-Bench (音频智能推理基准)**：音频推理性能评估基准。

## 数据集
- **VoiceAssistant-400K**：语音助手数据集，包含 400,000 条语音交互数据。
- **Benchmark 数据集**：
  - LLaMA Question
  - TrivialQA
  - ComplexBench
  - StepEval-Audio-360
- **数据集示例**：
  - **Librispeech**
  - **Common Voice**（包括 en, zh, yue, fr）
  - **Fleurs (zh)**
  - **Aishell2 (Mac/iOS/Android)**
  - **CoVoST2**（包括多种语言对，如 en-de, de-en, en-zh, zh-en, es-en, fr-en, it-en）
  - **Meld**
  - **VocalSound**
  - **Chat Benchmark**（Speech, Sound, Music, Mixed-Audio）
  - **合成数据**：MOSS dataset  
  - **Wenetspeech**
  - **CommonVoice**
  - **EMOBox**
  - **AirBench**
  - **SWAB**
  - **In-house testset**
  - **Seed-TTS**
  - **Web Questions**
  - **Llama Questions**
  - **TriviaQA**
  - **AlpacaEval**
  - **In-house ChitChat**
  - **Alimeeting**
  - **Fisher**
  - **Simulation**
  - **VoiceAssistant-400K**
  - **VCTK**
  - **Multilingual LibriSpeech**
  - **Libritts**
  - **Open-Orca**
  - **OpenAssistant**
  - **Trivia-Multichoice**
  - **Trivia-singlechoice**
  - **Rlhf**
  - **QAassistant**

## 任务与API
### API 参考
- **Qwen2-audio**  
  - [GitHub](https://github.com/QwenLM/Qwen2-Audio)
  - [HuggingFace Model](https://huggingface.co/Qwen/Qwen2-Audio-7B-Instruct)

- **Mini-Omni**  
  - [GitHub](https://github.com/gpt-omni/mini-omni)
  - 基于 Qwen2-0.5B 微调

- **MinMo (阿里巴巴通义)**  
  - [官网](https://funaudiollm.github.io/minmo/)
  - 支持用户实时打断交互，基于 Qwen2.5-7B-Instruct 微调

- **GLM-4-Voice**  
  - [GitHub](https://github.com/THUDM/GLM-4-Voice/tree/main)

- **Step-Audio-Chat (阶跃星辰)**  
  - [GitHub](https://github.com/stepfun-ai/Step-Audio)
  - [ModelScope](https://modelscope.cn/models/stepfun-ai/Step-Audio-Chat/files)

### Pipeline 说明
- **传统 ASR-LLM-TTS Pipeline**：传统的语音识别（ASR）模型与语言模型（LLM）和文本到语音（TTS）模块结合，形成的常见工作流程。
- **端到端 Pipeline**：通过将各模块的处理过程整合为一个统一的工作流，避免了中间步骤，提升了效率与响应速度。

### 模型架构
- **LLaMA-Omni**  
  - 将非自回归文本到语音模块与语言模型结合，使用连接时序损失函数（CTC loss）。
  
- **Freeze-Omni**  
  - 使用自回归与非自回归语音解码器的组合。

- **Minmo**  
  - 并行解码器结构，优势在于低延迟。

- **Moshi**  
  - 基于 Mini-Omni，适用于低延迟场景。

- **Emotion-aware interaction**  
  - **LUCY** 采用了 Mini-Omni（Xie & Wu，2024）的架构框架，并在对话数据集上进行了专门的微调，以实现情感控制和功能调用。

## 语音处理模型
### Tokenizer
- **Dual-codebook Speech Tokenizer**
  - 使用双代码本语音标记器将语音数据转换为可以处理的格式。
- **Step-Audio**  
  - 基于该模型，生成高质量的语音输出。
- **ARCON**  
  - 为语音识别与生成提供优化的多语言支持。
- **Linguistic Tokenizer**  
  - 对语音中的语言特征进行标记。
- **Paraformer Encoder**  
  - 用于语音编码的强大模型。
- **Semantic Tokenizer**  
  - 为语音生成提供更深层的语义理解。
- **CosyVoice Encoder**  
  - 优化了语音的语音风格与情感表达。

## 推荐硬件
- **H20 GPU**：支持高性能的语音生成任务。
- **A800 GPU**：适用于高负载的模型训练。

## 未来工作
- **情感识别与风格转换**：将继续完善情感控制与语音风格转换的精准度。
- **增强多语种支持**：进一步优化多语言与方言的支持，提供更自然的多模态交互。

<!-- ## 安装与使用
- 安装所需依赖：
  ```bash
  pip install -r requirements.txt -->