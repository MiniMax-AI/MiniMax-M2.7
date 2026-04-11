
<div align="center">
  <picture>
    <source srcset="figures/MiniMaxLogo-Dark.png" media="(prefers-color-scheme: dark)">
      <img src="figures/MiniMaxLogo-Light.png" width="60%" alt="MiniMax">
    </source>
  </picture>
</div>
<hr>

<div align="center" style="line-height: 1.4; font-size:16px; margin-top: 30px;">
  Join Our 
  <a href="https://platform.minimaxi.com/docs/faq/contact-us" target="_blank" style="font-size:17px; margin: 2px;">
    💬 WeChat
  </a> | 
  <a href="https://discord.com/invite/DPC4AHFCBw" target="_blank" style="font-size:17px; margin: 2px;">
    🧩 Discord
  </a> 
  community.
</div>
<div align="center" style="line-height: 1.2; font-size:16px;">
  <a href="https://agent.minimax.io/" target="_blank" style="display: inline-block; margin: 4px;">
    MiniMax Agent
  </a> | 
  <a href="https://platform.minimax.io/docs/guides/text-generation" target="_blank" style="display: inline-block; margin: 4px;">
    ⚡️ API
  </a> | 
  <a href="https://github.com/MiniMax-AI/MiniMax-MCP" style="display: inline-block; margin: 4px;">
    MCP
  </a> |
  <a href="https://www.minimax.io" target="_blank" style="display: inline-block; margin: 4px;">
    MiniMax Website
  </a> 
</div>
<div align="center" style="line-height: 1.2; font-size:16px; margin-bottom: 30px;">
  <a href="https://huggingface.co/MiniMaxAI" target="_blank" style="margin: 2px;">
    🤗 Hugging Face 
  </a> | 
  <a href="https://github.com/MiniMax-AI/MiniMax-M2.7" target="_blank" style="margin: 2px;">
    🐙 GitHub
  </a> | 
  <a href="https://www.modelscope.cn/organization/MiniMax" target="_blank" style="margin: 2px;">
    🤖️ ModelScope
  </a> | 
  <a href="https://github.com/MiniMax-AI/MiniMax-M2.7/blob/main/LICENSE" style="margin: 2px;">
    📄 LICENSE
  </a>
</div>

**MiniMax-M2.7** is our first model deeply participating in its own evolution. M2.7 is capable of building complex agent harnesses and completing highly elaborate productivity tasks, leveraging Agent Teams, complex Skills, and dynamic tool search. For more details, see our [blog post](https://www.minimax.io/news/minimax-m27-en).

<p align="center">
  <img width="100%" src="figures/benchmark_overview.png">
</p>

## Model Self-Evolution

M2.7 initiates a cycle of model self-evolution: during development, we let the model update its own memory, build dozens of complex skills for RL experiments, and improve its own learning process based on experiment results. An internal version of M2.7 autonomously optimized a programming scaffold over 100+ rounds — analyzing failure trajectories, modifying code, running evaluations, and deciding to keep or revert — achieving a **30% performance improvement**. On MLE Bench Lite (22 ML competitions), M2.7 achieved a **66.6% medal rate**, second only to Opus-4.6 and GPT-5.4.

<p align="center">
  <img width="100%" src="figures/agent_harness.png">
</p>

<p align="center">
  <img width="100%" src="figures/mle_bench.png">
</p>

## Professional Software Engineering

M2.7 delivers outstanding real-world programming capabilities spanning log analysis, bug troubleshooting, refactoring, code security, and machine learning. Beyond code generation, M2.7 demonstrates strong system-level reasoning — correlating monitoring metrics, conducting trace analysis, verifying root causes in databases, and making SRE-level decisions. Using M2.7, we have reduced live production incident recovery time to **under three minutes** on multiple occasions.

On SWE-Pro, M2.7 achieved **56.22%**, matching GPT-5.3-Codex, with even stronger performance on real-world engineering benchmarks: **SWE Multilingual (76.5)** and **Multi SWE Bench (52.7)**. On **VIBE-Pro (55.6%)**, M2.7 is nearly on par with Opus 4.6. On **Terminal Bench 2 (57.0%)** and **NL2Repo (39.8%)**, M2.7 demonstrates deep understanding of complex engineering systems. M2.7 also supports native **Agent Teams** for multi-agent collaboration with stable role identity and autonomous decision-making.

<p align="center">
  <img width="100%" src="figures/agent_teams.gif">
</p>

## Professional Work

M2.7 achieved an **ELO score of 1495** on GDPval-AA (highest among open-source models), surpassing GPT5.3. It handles Word, Excel, and PPT with high-fidelity multi-round editing, producing editable deliverables. On Toolathon, M2.7 reached **46.3%** accuracy (global top tier), and maintains **97% skill compliance** across 40+ complex skills on MM Claw. On the MM Claw end-to-end benchmark, M2.7 achieved **62.7%**, close to Sonnet 4.6.

## Entertainment

M2.7 features strengthened character consistency and emotional intelligence. We open-sourced [OpenRoom](https://github.com/MiniMax-AI/OpenRoom), an interactive demo that places AI interaction within a Web GUI space with real-time visual feedback and scene interactions. Try it at [openroom.ai](https://www.openroom.ai/).

## How to Use

- MiniMax Agent: https://agent.minimax.io/
- MiniMax API: https://platform.minimax.io/
- Token Plan: https://platform.minimax.io/subscribe/token-plan

## Local Deployment Guide

Download the model from HuggingFace repository: https://huggingface.co/MiniMaxAI/MiniMax-M2.7

We recommend using the following inference frameworks (listed alphabetically) to serve the model:

### SGLang

We recommend using [SGLang](https://docs.sglang.io/) to serve MiniMax-M2.7. Please refer to our [SGLang Deployment Guide](./docs/sglang_deploy_guide.md).

### vLLM

We recommend using [vLLM](https://github.com/vllm-project/vllm) to serve MiniMax-M2.7. Please refer to our [vLLM Deployment Guide](./docs/vllm_deploy_guide.md).

### Transformers

We recommend using [Transformers](https://github.com/huggingface/transformers) to serve MiniMax-M2.7. Please refer to our [Transformers Deployment Guide](./docs/transformers_deploy_guide.md).

### ModelScope

You also can get model weights from [modelscope](https://modelscope.cn/models/MiniMax/MiniMax-M2.7).

### NVIDIA NIM

MiniMax M2.7 is also available on [NVIDIA NIM Endpoint](https://build.nvidia.com).

### Inference Parameters

We recommend using the following parameters for best performance: `temperature=1.0`, `top_p = 0.95`, `top_k = 40`. Default system prompt:

```
You are a helpful assistant. Your name is MiniMax-M2.7 and is built by MiniMax.
```

## Tool Calling Guide

Please refer to our [Tool Calling Guide](./docs/tool_calling_guide.md).

## Contact Us

Contact us at [model@minimax.io](mailto:model@minimax.io).
