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
<!-- - [Popular Datasets](#available-datasets) -->

<!-- ## Datasets
<a id="Datasets"></a>
### Speech Interaction Datasets

- **Librispeech**: 1000 hours of English read speech at 16kHz. [[Link](https://www.openslr.org/12)]
- **Common Voice 15**: 7335 Hours,60 Languages[[Link](https://paperswithcode.com/dataset/common-voice)]
- **Fleurs**: 102 Languages,12 hours per language [[Link](https://huggingface.co/datasets/google/fleurs)]
- **Aishell2**: 1000 hours of clean read-speech data from iOS,Available for Mac/iOS/Android. [Link]
- **CoVoST2**: Multilingual dataset including English to multiple languages. [[Link](https://github.com/kaldi-asr/kaldi/tree/master/egs/aishell2)]
- **Meld**: Multimodal emotion dataset. MELD has more than 1400 dialogues and 13000 utterances from Friends TV series[[Link](https://affective-meld.github.io/)]
- **VocalSound**: 21,024 crowdsourced recordings of laughter, sighs, coughs, throat clearing, sneezes, and sniffs from 3,365 unique subjects[[Link](https://sls.csail.mit.edu/downloads/vocalsound/)]
- **Chat Benchmark**: Speech | Sound | Music | Mixed-Audio. [Link]
- **MOSS dataset**: Synthetic dataset[[Link](https://huggingface.co/datasets/YeungNLP/moss-003-sft-data)]
- **Wenetspeech**: 22400 hours[[Link](https://wenet.org.cn/WenetSpeech/)]
- **EMOBox**: Emotion-labeled dataset for speech. [[Link](https://github.com/emo-box/EmoBox)]
- **AirBench**: [Link]
- **SWAB**: [Link]

### In-house Test Datasets
- **Seed-TTS**: [Link] -->

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

<!-- ## Available Datasets
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
- **QAassistant** -->


# 语音数据集汇总
<a id="Datasets"></a>

## 1.Librispeech[[Link](https://www.openslr.org/12)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | English                                          |
| **语音类型** | 朗读、演讲                                       |
| **形式类型** | 非对话，单声道                                   |
| **总时长与数据集划分** | 总时长：约1000小时，分为 clean（较高质量）和 other（包含更多噪声）两类 |

---

## 2.Common Voice[[Link](https://paperswithcode.com/dataset/common-voice)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | English、Chinese、French、German等120种语言    |
| **语音类型** | 朗读，少量对话                                   |
| **形式类型** | 非对话，单声道（16kHz），极少部分双声道          |
| **总时长与数据集划分** | 总时长：约24000小时，英语占比最高（约 10,000+ 小时），中文约 3,000+ 小时 |

---

## 3.Fleurs[[Link](https://huggingface.co/datasets/google/fleurs)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | English、Chinese、French、German等102种语言    |
| **语音类型** | 新闻朗读                                         |
| **形式类型** | 非对话，单声道（16kHz）                          |
| **总时长与数据集划分** | 总时长：约12000小时，英语、中文、法语等每种语言300小时，大部分语种数据量严格均衡 |

---

## 4.Aishell2[[Link](https://github.com/kaldi-asr/kaldi/tree/master/egs/aishell2)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | Chinese                                          |
| **语音类型** | 朗读40%，自然对话60%                             |
| **形式类型** | 多人对话，多声道，单人对话，单声道               |
| **总时长与数据集划分** | 总时长：约1000小时，面向智能家居与移动端语音交互，跨设备录制，包含手机、平板、智能音箱、iOS、Android、Mac等 |

---

## 5.CoVoST2[[Link](https://paperswithcode.com/dataset/covost2)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | 覆盖了21种语言到英语和从英语到15种语言的数据库，包括法语、德语、荷兰语、俄语、西班牙语、意大利语等 |
| **语音类型** | 朗读                                             |
| **形式类型** | 非对话，单声道（16kHz）                          |
| **总时长与数据集划分** | 总时长：约2880小时，采用 Common Voice 数据库中的语音录音创建 |

---

## 6.Meld[[Link](https://affective-meld.github.io/)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | 英语 |
| **语音类型** | 电影中的对话                                             |
| **形式类型** | 对话，单声道                          |
| **总时长与数据集划分** | 总时长：约29小时，源自电视剧《老友记》，1,400 个对话和 13,000 个句子。这些对话涉及多个 speaker，对话中的每个句子都被标记为七种情绪中的其中一种： 愤怒、厌恶、悲伤、快乐、中立、惊讶和恐惧 |

---

## 7.VocalSound[[Link](https://sls.csail.mit.edu/downloads/vocalsound/)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | 英语 |
| **语音类型** | 非对话音频                                            |
| **形式类型** | 非对话，单声道                          |
| **总时长与数据集划分** | 音频长度的平均值是4.18秒，总时长：23小时，包含 3,365 名不同受试者的 21,024 条众包录音，包括笑声、叹气声、咳嗽声、清嗓子声、打喷嚏声和吸气声 |

---

## 8.Wenetspeech[[Link](https://wenet.org.cn/WenetSpeech/)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | 中文 |
| **语音类型** | 有声读物，现场解说，纪录片，戏剧，采访，新闻，阅读，讨论，综艺                                            |
| **形式类型** | 单声道                          |
| **总时长与数据集划分** | 总时长：10000+小时，数据均来自 YouTube 和 Podcast |

---

## 9.EMOBox[[Link](https://github.com/emo-box/EmoBox)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | 涵盖14种不同的语言，包括12个英语数据集、3个普通话数据集，以及各2个法语、德语和意大利语数据集。此外，阿姆哈拉语、孟加拉语、希腊语、波斯语、波兰语、俄语、西班牙语、土耳其语和乌尔都语各有1个数据集 |
| **语音类型** | 访谈、对话、演讲、辩论、朗读                                            |
| **形式类型** | 单声道                          |
| **总时长与数据集划分** | 总时长：294.4小时 |

---

## 10.AirBench[[Link](https://github.com/emo-box/EmoBox)]

| **属性**     | **内容**                                         |
|--------------|--------------------------------------------------|
| **语种**     | English, Chinese, Spanish, French, German, Russian, Japanese, Korean, Arabic, Persian, Indonesian, Hindi, Bengali |
| **语音类型** |                                             |
| **形式类型** |                           |
| **总时长与数据集划分** |  |

---
