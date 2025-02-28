# End-to-End Speech Interaction Research

This repository collects common datasets, APIs, and papers related to the research on end-to-end speech interaction, including ASR, S2TT, emotion-aware interaction, and voice style conversion.

This repository is continuously updating🎉

<!-- If this repository brings you some inspiration, I would be very honored😊 -->

<!-- If you have any suggestions, feel free to contact me with: your-email@example.com📮 -->

<!-- Additionally, if you could consider giving my repository a star🌟, that would motivate me a lot! -->

## Contents

- [Datasets](#Datasets)
- [End-to-End Speech Interaction APIs](#paper)
- [Pipelines](#pipelines)
- [Popular Datasets](#available-datasets)

## Datasets
<a id="Datasets"></a>
### Speech Interaction Datasets

- **Librispeech**: 1000 hours of English read speech at 16kHz. [Link]
- **Common Voice 15**: Multiple languages including English, Chinese, Cantonese, and French. [Link]
- **Fleurs**: Focused on Chinese. [Link]
- **Aishell2**: Available for Mac/iOS/Android. [Link]
- **CoVoST2**: Multilingual dataset including English to multiple languages. [Link]
- **Meld**: Multimodal emotion dataset. [Link]
- **VocalSound**: [Link]
- **Chat Benchmark**: Speech | Sound | Music | Mixed-Audio. [Link]
- **Synthetic Data**: MOSS dataset. [Link]
- **Wenetspeech**: [Link]
- **CommonVoice**: Another large-scale voice dataset. [Link]
- **EMOBox**: Emotion-labeled dataset for speech. [Link]
- **AirBench**: [Link]
- **SWAB**: [Link]

### In-house Test Datasets
- **Seed-TTS**: [Link]

## End-to-End Speech Interaction APIs
<a id="paper"></a>

### [Qwen2-Audio](https://github.com/QwenLM/Qwen2-Audio)
- Hugging Face Model: [Qwen2-Audio-7B-Instruct](https://huggingface.co/Qwen/Qwen2-Audio-7B-Instruct)

### [Mini-Omni](https://github.com/gpt-omni/mini-omni)
- Fine-tuned on Qwen2-0.5B

### [MinMo (通义)](https://funaudiollm.github.io/minmo/)
- Real-time interruption interaction support
- Fine-tuned on Qwen2.5-7B-Instruct

### [GLM-4-Voice](https://github.com/THUDM/GLM-4-Voice/tree/main)

### [Step-Audio-Chat (阶跃星辰)](https://github.com/stepfun-ai/Step-Audio)
- Model: [Step-Audio-Chat](https://modelscope.cn/models/stepfun-ai/Step-Audio-Chat/files)

## Pipelines
<a id="pipelines"></a>

- **ASR-LLM-TTS**: Traditional pipeline combining ASR, LLM, and TTS.
- **End-to-End Pipelines**: Non-autoregressive text-to-speech models with language models using connectionist temporal loss.

<!-- ## Emotion-Aware Interaction

### LUCY
- Based on Mini-Omni's architecture, specifically fine-tuned for emotion control and function calling. -->

## Available Datasets
<a id="available-datasets"></a>

- **Librispeech**
- **Common Voice 15**: English, Chinese, Cantonese, French
- **Fleurs**: Chinese
- **Aishell2**: Mac/iOS/Android
- **CoVoST2**: en-de | de-en | en-zh | zh-en | es-en | fr-en | it-en
- **Meld**
- **VocalSound**
- **Chat Benchmark**: Speech | Sound | Music | Mixed-Audio
- **Synthetic Datasets**: MOSS dataset
- **Wenetspeech**
- **CommonVoice**
- **EMOBox**
- **AirBench**
- **SWAB**
- **Seed-TTS**
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
- **Trivia-Singlechoice**
- **Rlhf**
- **QAassistant**