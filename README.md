# Setup Guide

Based on [AudioToText GitHub Repository](https://github.com/Carleslc/AudioToText)

This Jupyter notebook uses the original Whisper model, which is slower than `whisper.cpp` or `fasterwhisper`.

## 1. Build the Virtual Environment (venv) with `uv`
```bash
uv venv --python 3.12
```


	
## 2. Install `whisper` and dependencies
```bash
uv pip install openai numpy scipy deepl pydub cohere ffmpeg-python tensorflow-probability typing-extensions
uv pip install git+https://github.com/openai/whisper.git
uv pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
# for vscode jupyter
uv pip install ipykernel
```

