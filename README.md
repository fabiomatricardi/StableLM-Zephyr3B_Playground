# StableLM-Zephyr3B_Playground
Repo for the code to create a Playground for StablLM-Zephyr-3B GGUF with Gradio

<img src="https://github.com/fabiomatricardi/StableLM-Zephyr3B_Playground/raw/main/logo-banner-StableZephyr.jpg" width=300>

Only requirements:
```
pip install llama-cpp-python==0.2.20
pip install gradio
```

- Model Context lenght is 4096 tokens
- stop-word = ["</s>"]

This model does not have a System message in the prompt

### Prompt template: StableLM-Zephyr
```
<|user|>
{prompt}<|endoftext|>
<|assistant|>
```
To use it in a f-string:
```python
prompt = f"<|user|>\n{prompt}<|endoftext|>\n<|assistant|>"
```

### Result
<img src="https://github.com/fabiomatricardi/StableLM-Zephyr3B_Playground/raw/main/stablelm-zephyr3B-finalGUI.png" width=800>
