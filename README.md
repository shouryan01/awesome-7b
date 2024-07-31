# awesome-7b

Tracking the best open-source llms that can *actually* run on consumer-level hardware.

<br />

## Tiny Models (recommended for mobile)
(model sizes <=6b) 

| Name | Size | Context Length | Weights | Ollama |
|---|---|---|---|---|
| Gemma 2 | 2B | 8k | [🤗 HF](https://huggingface.co/google/gemma-2-2b-it) | [Model](https://ollama.com/library/gemma2:2b)
| Phi-3 Mini | 3.8B | 4k (128k available) | [🤗 HF](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct) | [Model](https://ollama.com/library/phi3:3.8b)


## Small Models (recommended for desktop)
(model sizes 7b-10b) 

| Name | Size | Context Length | Weights | Ollama |
|---|---|---|---|---|
| Mistral v0.3 | 7.3B | 32k | [🤗 HF](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.3) | [Model](https://ollama.com/library/mistral:7b)
| Llama 3.1 | 8B | 128k | [🤗 HF](https://huggingface.co/meta-llama/Meta-Llama-3.1-8B-Instruct) | [Model](https://ollama.com/library/llama3.1:8b)
| Gemma 2 | 9B | 8k | [🤗 HF](https://huggingface.co/google/gemma-2-9b-it) | [Model](https://ollama.com/library/gemma2:9b)

## Medium Models
(model sizes 11b-16b)

| Name | Size | Context Length | Weights | Ollama |
|---|---|---|---|---|
| Mistral NeMo | 12B | 128k | [🤗 HF](https://huggingface.co/mistralai/Mistral-Nemo-Instruct-2407) | [Model](https://ollama.com/library/mistral-nemo)

## Large Models
(model sizes 17b-33b)

| Name | Size | Context Length | Weights | Ollama |
|---|---|---|---|---|
| Gemma 2 | 27B | 8k | [🤗 HF](https://huggingface.co/google/gemma-2-27b-it) | [Model](https://ollama.com/library/gemma2:27b)

## Huge Models (not for GPU-poor)
(model sizes >33b)
| Name | Size | Context Length | Weights | Ollama |
|---|---|---|---|---|
| Llama 3.1 | 70B | 128k | [🤗 HF](https://huggingface.co/meta-llama/Meta-Llama-3.1-70B) | [Model](https://ollama.com/library/llama3.1:70b)

<br />

## FAQ

### What makes a model "good"?
<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I pretty much only trust two LLM evals right now: Chatbot Arena and r/LocalLlama comments section</p>&mdash; Andrej Karpathy (@karpathy) <a href="https://twitter.com/karpathy/status/1737544497016578453?ref_src=twsrc%5Etfw">December 20, 2023</a></blockquote>

[r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA) discussions and [Chatbot Arena](https://chat.lmsys.org/)

Don't trust benchmarks. Download the model and decide for yourself. Models are free so there's no downside lol.

### What's Ollama and why should I use it?
[Ollama](https://ollama.com/) just makes using LLMs that much more accessible for beginners. It's built on top of [llama.cpp](https://github.com/ggerganov/llama.cpp) and is [FOSS](https://github.com/ollama/ollama).

### Which model should I use?
This one depends on *you*. How powerful is your hardare? How complicated is your use-case? A **small** model should is a good starting point. Then, if you need more speed you look at smaller models; if you need more power you turn to larger ones.

### What does "size" mean?
It means how powerful the model is, how large the download size will be, and how much system resources you will need. According to [Ollama](https://github.com/ollama/ollama#:~:text=You%20should%20have%20at%20least%208%20GB%20of%20RAM%20available%20to%20run%20the%207B%20models%2C%2016%20GB%20to%20run%20the%2013B%20models%2C%20and%2032%20GB%20to%20run%20the%2033B%20models.): You should have at least 8 GB of RAM available to run the 7B models, 16 GB to run the 13B models, and 32 GB to run the 33B models.

### What does "context length" mean?
It refers to how long your prompts to the LLM can be. Higher is better (but may be slower and lower quality).

### Which quant should I use?
If you don't know what `quant` means, ignore this question. If you do, the largest your computer can handle. For most people, that's `q5_K_M`. Ollama's default is `q4_0`.




