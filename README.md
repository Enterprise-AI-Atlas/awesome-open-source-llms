# Awesome Open-Source LLMs

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)

A curated, category-organized registry of open-weight / open-source large language models (LLMs), vision-language models, and related model families.

The goal is to be the definitive place to discover downloadable foundation models you can run locally, fine-tune, or embed in your own products.

**Inclusion criteria:** Models must ship publicly downloadable weights with a clear open-source or open-weight license. Closed API-only models are out of scope. See [CONTRIBUTING.md](./CONTRIBUTING.md) for the full quality bar.

---

## Contents

- [General-Purpose LLMs](#general-purpose-llms)
- [Coding LLMs](#coding-llms)
- [Reasoning LLMs](#reasoning-llms)
- [Small / Fast LLMs](#small--fast-llms)
- [Multilingual LLMs](#multilingual-llms)
- [Vision-Language Models](#vision-language-models)
- [Fine-Tuned Variants](#fine-tuned-variants)
- [Model Families / Hugging Face Collections](#model-families--hugging-face-collections)
- [License Notes](#license-notes)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

---

## General-Purpose LLMs

Large, general-capability text models suitable for chat, RAG, agents, and long-context tasks.

- **[Llama 3.1 Instruct](https://huggingface.co/collections/meta-llama/llama-31)** `Official` — Meta's dense instruction-tuned flagship family.
  - Sizes: 8B, 70B, 405B
  - License: [Llama 3.1 License](https://www.llama.com/llama3/license/)
- **[Llama 3.2 Instruct](https://huggingface.co/collections/meta-llama/llama-32)** `Official` — Lightweight, multilingual Llama models with vision variants.
  - Sizes: 1B, 3B
  - License: [Llama 3.2 License](https://www.llama.com/llama3/license/)
- **[Mistral Large 2](https://huggingface.co/mistralai/Mistral-Large-Instruct-2407)** `Official` — Production-grade general-purpose model with a 128K context window.
  - Sizes: ~123B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Mistral 7B Instruct v0.3](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.3)** `Official` — Efficient 7B Apache 2.0 model popular for local deployment.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Qwen2.5 Instruct](https://huggingface.co/collections/Qwen/qwen25)** `Official` — Alibaba's dense instruction-tuned family covering a wide parameter range.
  - Sizes: 0.5B, 1.5B, 3B, 7B, 14B, 32B, 72B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[Qwen3](https://huggingface.co/Qwen/Qwen3-235B-A22B)** `Official` — Latest Qwen3 flagship MoE with hybrid reasoning modes.
  - Sizes: 0.6B–235B-A22B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[DeepSeek-V3](https://huggingface.co/deepseek-ai/DeepSeek-V3)** `Official` — MoE frontier model competitive with leading closed-source LLMs.
  - Sizes: 671B total / 37B active
  - License: [DeepSeek License](https://github.com/deepseek-ai/DeepSeek-V3/blob/main/LICENSE-MODEL)
- **[Gemma 2](https://huggingface.co/collections/google/gemma-2-release)** `Official` — Lightweight, high-quality open models by Google DeepMind.
  - Sizes: 2B, 9B, 27B
  - License: [Gemma Terms of Use](https://ai.google.dev/gemma/terms)
- **[Phi-4](https://huggingface.co/microsoft/phi-4)** `Official` — Microsoft's state-of-the-art dense model for reasoning and language tasks.
  - Sizes: 14B
  - License: [MIT](https://opensource.org/license/mit)
- **[Yi-1.5](https://huggingface.co/collections/01-ai/yi-15-664fff4adca44be04076bafc)** `Official` — 01.AI's bilingual base and chat model family.
  - Sizes: 6B, 9B, 34B
  - License: [Yi License](https://github.com/01-ai/Yi/blob/main/LICENSE)

---

## Coding LLMs

Models fine-tuned or pre-trained specifically for code generation, completion, infilling, and software engineering tasks.

- **[Code Llama](https://huggingface.co/collections/meta-llama/code-llama-family)** `Official` — Meta's code-specialized Llama 2 family.
  - Sizes: 7B, 13B, 34B, 70B
  - License: [Llama 2 License](https://www.llama.com/llama2/license/)
- **[DeepSeek-Coder-V2](https://huggingface.co/deepseek-ai/DeepSeek-Coder-V2-Instruct-0724)** `Official` — MoE code model with strong multi-language performance.
  - Sizes: 236B total / 21B active
  - License: [DeepSeek License](https://github.com/deepseek-ai/DeepSeek-Coder-V2/blob/main/LICENSE-MODEL)
- **[Codestral](https://huggingface.co/mistralai/Codestral-22B-v0.1)** `Official` — Mistral's 22B fill-in-the-middle coding model.
  - Sizes: 22B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Qwen2.5-Coder](https://huggingface.co/collections/Qwen/qwen25-coder)** `Official` — Code-specific Qwen models covering many sizes.
  - Sizes: 0.5B, 1.5B, 3B, 7B, 14B, 32B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[StarCoder2](https://huggingface.co/collections/bigcode/starcoder2-65de6a6edb6df0d7ef5c5df9)** `Official` — Transparently trained code generation model by BigCode.
  - Sizes: 3B, 7B, 15B
  - License: [BigCode OpenRAIL-M](https://huggingface.co/spaces/bigcode/license)
- **[Magicoder-S-DS-6.7B](https://huggingface.co/ise-uiuc/Magicoder-S-DS-6.7B)** `Community` — OSS-Instruct distilled coding model.
  - Sizes: 6.7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)** `Official` — Qwen 1.5 code model with long-context support.
  - Sizes: 7B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[Granite Code](https://huggingface.co/collections/ibm-granite/granite-code-models-6624c1dec90119f90b100d96)** `Official` — IBM's enterprise-focused code model family.
  - Sizes: 3B, 8B, 20B, 34B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)

---

## Reasoning LLMs

Models optimized for chain-of-thought reasoning, math, science, and complex problem solving.

- **[DeepSeek-R1](https://huggingface.co/deepseek-ai/DeepSeek-R1)** `Official` — Open reasoning model trained with reinforcement learning, plus distillations.
  - Sizes: 671B / distilled 1.5B–70B
  - License: [DeepSeek License](https://github.com/deepseek-ai/DeepSeek-R1/blob/main/LICENSE)
- **[DeepSeek-R1-Distill-Qwen-32B](https://huggingface.co/deepseek-ai/DeepSeek-R1-Distill-Qwen-32B)** `Official` — Distilled reasoning model combining DeepSeek-R1 outputs with Qwen.
  - Sizes: 32B
  - License: [DeepSeek License / Qwen License](https://github.com/deepseek-ai/DeepSeek-R1/blob/main/LICENSE)
- **[QwQ-32B-Preview](https://huggingface.co/Qwen/QwQ-32B-Preview)** `Official` — Qwen reasoning model preview with strong math and logic performance.
  - Sizes: 32B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[Skywork-o1-Open-Llama-8B](https://huggingface.co/Skywork/Skywork-o1-Open-Llama-8B)** `Official` — Open reasoning model from the Skywork series.
  - Sizes: 8B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[OpenThinker-7B](https://huggingface.co/open-thoughts/OpenThinker-7B)** `Community` — Reasoning model trained on the Open Thoughts dataset.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Marco-o1](https://huggingface.co/AIDC-AI/Marco-o1)** `Community` — Reasoning model focused on real-world problem solving.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)

---

## Small / Fast LLMs

Compact models designed for edge, mobile, low-latency, or CPU/GPU-constrained deployments.

- **[Phi-4-mini-instruct](https://huggingface.co/microsoft/Phi-4-mini-instruct)** `Official` — Small reasoning-capable model from Microsoft.
  - Sizes: 3.8B
  - License: [MIT](https://opensource.org/license/mit)
- **[Gemma 2 2B IT](https://huggingface.co/google/gemma-2-2b-it)** `Official` — Tiny on-device instruction-tuned model.
  - Sizes: 2B
  - License: [Gemma Terms of Use](https://ai.google.dev/gemma/terms)
- **[Qwen2.5-0.5B-Instruct](https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct)** `Official` — Sub-billion instruction model for edge use cases.
  - Sizes: 0.5B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[Llama 3.2 1B Instruct](https://huggingface.co/meta-llama/Llama-3.2-1B-Instruct)** `Official` — Edge-friendly multilingual instruction model.
  - Sizes: 1B
  - License: [Llama 3.2 License](https://www.llama.com/llama3/license/)
- **[SmolLM2 Instruct](https://huggingface.co/collections/HuggingFaceTB/smollm2-6728b3b31ef5fbed4d1e2c25)** `Official` — Hugging Face small-language-model family.
  - Sizes: 135M, 360M, 1.7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[TinyLlama-1.1B-Chat](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0)** `Community` — 1.1B chat model trained on 3T tokens.
  - Sizes: 1.1B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[MiniCPM3-4B](https://huggingface.co/openbmb/MiniCPM3-4B)** `Official` — 4B model with performance rivaling many 7B models.
  - Sizes: 4B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Gemma 2B IT](https://huggingface.co/google/gemma-2b-it)** `Official` — First-generation Gemma on-device instruction model.
  - Sizes: 2B
  - License: [Gemma Terms of Use](https://ai.google.dev/gemma/terms)

---

## Multilingual LLMs

Models explicitly trained or evaluated for strong performance across many languages.

- **[Aya 23](https://huggingface.co/collections/CohereForAI/aya-23-6641ebf63345c7ebd9dbca57)** `Official` — Cohere's multilingual family covering 23 languages.
  - Sizes: 8B, 35B
  - License: [See model card](https://huggingface.co/CohereForAI/aya-23-35b)
- **[Aya Expanse](https://huggingface.co/collections/CohereForAI/aya-expanse-66cd6693ef91343f0e86696e)** `Official` — Improved multilingual instruction model.
  - Sizes: 8B, 32B
  - License: [See model card](https://huggingface.co/CohereForAI/aya-expanse-32b)
- **[BLOOM](https://huggingface.co/bigscience/bloom)** `Official` — Multilingual LLM developed by the BigScience workshop.
  - Sizes: 560M–176B
  - License: [BigScience RAIL License](https://bigscience.huggingface.co/blog/the-bigscience-rail-license)
- **[XGLM](https://huggingface.co/facebook/xglm-7.5B)** `Official` — Meta's multilingual model trained on 30 languages.
  - Sizes: 7.5B
  - License: [See model card](https://huggingface.co/facebook/xglm-7.5B)
- **[SeaLLM](https://huggingface.co/SeaLLMs/SeaLLM-7B-v2)** `Official` — Southeast Asian language model.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Yi-1.5-34B-Chat](https://huggingface.co/01-ai/Yi-1.5-34B-Chat)** `Official` — Strong Chinese-English bilingual chat model.
  - Sizes: 34B
  - License: [Yi License](https://github.com/01-ai/Yi/blob/main/LICENSE)

---

## Vision-Language Models

Open models that jointly process text and images for captioning, visual QA, OCR, and multimodal agents.

- **[LLaVA 1.6 34B](https://huggingface.co/liuhaotian/llava-v1.6-34b)** `Community` — Visual instruction-tuned large multimodal model.
  - Sizes: 34B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Qwen2-VL 7B Instruct](https://huggingface.co/Qwen/Qwen2-VL-7B-Instruct)** `Official` — Vision-language model with multilingual OCR and grounding.
  - Sizes: 7B
  - License: [Apache 2.0 / Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)
- **[InternVL2 8B](https://huggingface.co/OpenGVLab/InternVL2-8B)** `Official` — Open-source vision foundation model.
  - Sizes: 8B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[PaliGemma 3B](https://huggingface.co/google/paligemma-3b-pt-224)** `Official` — Google's 3B vision-language model.
  - Sizes: 3B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[MiniCPM-V 2.6](https://huggingface.co/openbmb/MiniCPM-V-2_6)** `Official` — Efficient vision-language model with strong OCR.
  - Sizes: 8B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Moondream 2](https://huggingface.co/vikhyatk/moondream2)** `Community` — Tiny vision-language model for edge devices.
  - Sizes: 1.6B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Idefics3 8B](https://huggingface.co/HuggingFaceM4/Idefics3-8B-Llama3)** `Official` — Multimodal model by Hugging Face M4.
  - Sizes: 8B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Bunny-v1.0-4B](https://huggingface.co/BAAI/Bunny-v1_0-4B)** `Community` — Compact vision-language model from BAAI.
  - Sizes: 4B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)

---

## Fine-Tuned Variants

Popular community and research fine-tunes built on top of open foundation models.

- **[Dolphin 2.9 Llama 3.1 70B](https://huggingface.co/cognitivecomputations/dolphin-2.9.4-llama-3.1-70b)** `Community` — General chat fine-tune of Llama 3.1.
  - Sizes: 70B
  - License: [Llama 3.1 License](https://www.llama.com/llama3/license/)
- **[Nous Hermes 2 Yi 34B](https://huggingface.co/NousResearch/Nous-Hermes-2-Yi-34B)** `Community` — General-purpose Yi fine-tune.
  - Sizes: 34B
  - License: [Yi License](https://github.com/01-ai/Yi/blob/main/LICENSE)
- **[Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)** `Community` — RLHF-tuned chat model.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[OpenChat 3.5](https://huggingface.co/openchat/openchat-3.5-0106)** `Community` — General-purpose conversation fine-tune.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Neural Chat 7B v3](https://huggingface.co/Intel/neural-chat-7b-v3-1)** `Official` — Intel supervised fine-tune of Mistral 7B.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Tülu 3 70B](https://huggingface.co/allenai/llama-3-tulu-3-70b)** `Official` — AI2's instruction-following model suite.
  - Sizes: 70B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **[Vicuna 13B v1.5](https://huggingface.co/lmsys/vicuna-13b-v1.5)** `Community` — Early open chat fine-tune of Llama 2.
  - Sizes: 13B
  - License: [Llama 2 License](https://www.llama.com/llama2/license/)
- **[Zephyr 7B beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)** `Official` — Hugging Face H4 direct preference optimization fine-tune.
  - Sizes: 7B
  - License: [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)

---

## Model Families / Hugging Face Collections

Curated starting points for browsing full model families and official collections on the Hugging Face Hub.

- **[Meta Llama 3.1 Collection](https://huggingface.co/collections/meta-llama/llama-31)** `Official` — All Llama 3.1 base, instruct, and guard models.
- **[Mistral AI Organization](https://huggingface.co/mistralai)** `Official` — Mistral, Mixtral, Codestral, and embedding models.
- **[Qwen2.5 Collection](https://huggingface.co/collections/Qwen/qwen25)** `Official` — Dense and instruction-tuned Qwen2.5 checkpoints.
- **[Google Gemma 2 Collection](https://huggingface.co/collections/google/gemma-2-release)** `Official` — Gemma 2 base and instruction-tuned models.
- **[Microsoft Phi-4 Collection](https://huggingface.co/collections/microsoft/phi-4-66e9971ab7f5f6f2c97c085b)** `Official` — Phi-4 and Phi-4-mini models.
- **[DeepSeek Organization](https://huggingface.co/deepseek-ai)** `Official` — DeepSeek-V3, DeepSeek-Coder, and DeepSeek-R1 families.
- **[Allen AI OLMo 2 Collection](https://huggingface.co/collections/allenai/olmo-2-66cf51e435ecab9b11a884d9)** `Official` — Truly open-source training-data-and-all language models.
- **[NVIDIA Llama-3.1-Nemotron Collection](https://huggingface.co/collections/nvidia/llama-31-nemotron-51-66b8ad9220d8c7b8c1d0c0ec)** `Official` — NVIDIA's Llama 3.1 Nemotron fine-tunes for helpfulness and reward modeling.

---

## License Notes

Open-weight LLMs are released under a variety of licenses. Always review the model card before deploying commercially.

- **[Llama 3.x License](https://www.llama.com/llama3/license/)** — Meta's custom license for Llama 3.1, 3.2, and 3.3 models.
- **[Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)** — Permissive license used by Qwen, Mistral Large 2, Gemma 2, and many others.
- **[MIT](https://opensource.org/license/mit)** — Very permissive license used by Microsoft Phi models.
- **[BigCode OpenRAIL-M](https://huggingface.co/spaces/bigcode/license)** — Responsible AI license used by StarCoder2.
- **[BigScience RAIL License](https://bigscience.huggingface.co/blog/the-bigscience-rail-license)** — License for the BLOOM family.
- **[DeepSeek License](https://github.com/deepseek-ai/DeepSeek-V3/blob/main/LICENSE-MODEL)** — Custom license for DeepSeek-V3, Coder-V2, and R1.
- **[Gemma Terms of Use](https://ai.google.dev/gemma/terms)** — Google's terms for Gemma models.
- **[Qwen License](https://github.com/QwenLM/Qwen/blob/main/LICENSE)** — Alibaba's license supplement for some Qwen releases.
- **[Yi License](https://github.com/01-ai/Yi/blob/main/LICENSE)** — 01.AI's custom license for the Yi family.

---

## Related Awesome Lists

- **[Awesome Local LLMs](https://github.com/vince-lam/awesome-local-llms)** — Tools and resources for running LLMs locally.
- **[Awesome CLI Coding Agents](https://github.com/bradAGI/awesome-cli-coding-agents)** — Terminal-native AI coding agents and harnesses.
- **[Cloud GPUs](https://github.com/cloud-gpus/cloud-gpus.github.io)** — Comparison site and data for cloud GPU instances.

---

## Contributing

Read [CONTRIBUTING.md](./CONTRIBUTING.md) for the quality bar, entry format, and PR process.

---

## License

This list is released into the public domain under [CC0-1.0](./LICENSE).

## Want us to build this for you?

Enterprise AI Atlas is maintained by [Vibe Coding Agency](https://vibecodingagency.com). We prototype and ship agentic systems, MCP servers, and enterprise AI integrations for teams that need working software fast — without hiring a full AI engineering team.
