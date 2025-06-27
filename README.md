# Hey there, I’m **VJHack** 👋

**Fast, hermetic builds with Bazel** · **LLM inference & optimisation**

---

I'm a software engineer passionate about builds and AI. <br>
With Bazel, there's no reason not to have lightning-fast, cross-platform builds. <br>
I believe everyone should be able to run language models on consumer hardware, and I'm deeply interested in inference and performance optimization.

---

### Major Contributions

#### **ggml‑org / llama.cpp**
- [#11223 – Top‑σ sampler](https://github.com/ggml-org/llama.cpp/pull/11223) | [Paper](https://arxiv.org/pdf/2411.07641v1) – Implemented Top‑σ sampling algorithm from the paper Top-nσ: Not All Logits Are You Need, a novel alternative to Top‑k/Top‑p for LLM decoding, creating a stable sampling space even in high temeratures.
- [#11180](https://github.com/ggml-org/llama.cpp/pull/11180) [#11116](https://github.com/ggml-org/llama.cpp/pull/11116) – Restructures the gguf PyPI package to avoid installing multiple top-level packages and prevent conflicts with existing scripts directory.
-  – Fixed memory alignment issues in quantized KV-cache allocations, improving stability for int4 models.
- [#9527](https://github.com/ggml-org/llama.cpp/pull/9527) – Updates `response_format` to match OpenAI's new structured output schema
- [#9484](https://github.com/ggml-org/llama.cpp/pull/9484) – Added the option to disable context shift on infinite text generation with command line argument (`--no-context-shift`) 

#### **ggml‑org / llama.vim**
- [#15](https://github.com/ggml-org/llama.vim/pull/15) – Adds a local cache for FIM completions to reduce server calls. Uses a SHA-256 hash of the prompt state as the key. Default size is 250 (configurable), with a random eviction policy.
- [#18](https://github.com/ggml-org/llama.vim/pull/18) – Optimizes FIM cache by retaining suggestions when the user continues typing the same text.
- [#21](https://github.com/ggml-org/llama.vim/pull/21) – Updates the info message to show cache-specific metrics on cache hits (`C: current/size | t: total time`). Also reduces cache size by storing only the completion content.
- [#24](https://github.com/ggml-org/llama.vim/pull/24) – Minimizes server-client payloads by filtering out unused response fields. Applies to both `ring_update()` and main FIM calls, keeping only essential fields like content and timings. 

---


