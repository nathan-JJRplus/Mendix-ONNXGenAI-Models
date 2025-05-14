# Pre-built models for usage with ONNXRuntime-GenAI
These models are optimized for usage on the Mendix runtime and are plug-and-play for the GenAI marketplace module (W.I.P.)

All of the models are built using Olive auto-opt and are optimized for inference on CPU, with int4 quantization for minimal memory usage

Example command:

```
olive auto-opt --model_name_or_path deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B --output_path ./deepseek-r1-distill-qwen-1.5B --device cpu --provider CPUExecutionProvider --precision int4 --use_model_builder --log_level 1
```

## Current library

### Deepseek-R1-distill-qwen-1.5b
- Commercial use? ✅
- Model size ~1.83gb
- [Source](https://huggingface.co/deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B)

### Gemma3
- Commercial use? ❌
- Model size ~1.76gb
- [Source](https://huggingface.co/google/gemma-3-1b-it)

### Phi-1
- Commercial use? ✅
- Model size ~1.16gb
- [Source](https://huggingface.co/microsoft/phi-1)

### Phi-1.5
- Commercial use? ✅
- Model size ~1.16gb
- [Source](https://huggingface.co/microsoft/phi-1_5)

### Phi-2
- Commercial use? ✅
- Model size ~2.03gb
- [Source](https://huggingface.co/microsoft/phi-2)

### Qwen1.5-0.5B-Chat
- Commercial use? ❌
- Model size ~878mb
- [Source](https://huggingface.co/Qwen/Qwen1.5-0.5B-Chat)

### TinyLLama
- Commercial use? ✅
- Model size ~876mb
- [Source](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0)

## Want a different model?
Build it yourself using the ONNXRuntime-GenAI package [Tutorial](https://onnxruntime.ai/docs/genai/howto/build-model.html)

Or, open a ticket in this repo, and I'll see what I can do 😄