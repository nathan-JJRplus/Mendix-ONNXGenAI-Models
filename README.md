# Pre-built models for usage with ONNXRuntime-GenAI
These models are optimized for usage on the Mendix runtime and are plug-and-play for the GenAI marketplace module (W.I.P.)

All of the models are built using Olive auto-opt and are optimized for inference on CPU, with int4 quantization for minimal memory usage

Example command:

```
olive auto-opt --model_name_or_path deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B --output_path ./deepseek-r1-distill-qwen-1.5B --device cpu --provider CPUExecutionProvider --precision int4 --use_model_builder --log_level 1
```

## Current library

### Deepseek-R1-distill-qwen-1.5b
- [Huggingface](https://huggingface.co/deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B)
- Model size ~1.83gb
### Gemma3
- [Huggingface](https://huggingface.co/google/gemma-3-1b-it)
- Model size ~1.76gb
### Phi-2
- [Huggingface](https://huggingface.co/microsoft/phi-2)
- Model size ~2.03gb
### TinyLLama
- [Huggingface](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0)
- Model size ~876mb

## Contribution
If you want to add a model you've prebuilt to this library please make sure to include relative paths in `model_config.json` for `"model_path"` and `"additional_files"` 