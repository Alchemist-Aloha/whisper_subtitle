# Setup Guide

2025/03/09 Check my [explicit_util](https://github.com/Alchemist-Aloha/explicit_util). The transcription is now utilizing whisper.cpp and is almost 100% faster. 

Based on [AudioToText GitHub Repository](https://github.com/Carleslc/AudioToText)

This Jupyter notebook uses the original Whisper model, which is slower than `whisper.cpp` or `fasterwhisper`.

## 1. Build the Virtual Environment (venv) with `uv`
```bash
uv venv --python 3.12
.venv\Scripts\activate
```


	
## 2. Install `whisper` and dependencies
```bash
uv pip install -r requirements.txt
```

or

```bash
uv pip install openai numpy scipy pydub cohere ffmpeg-python tensorflow-probability typing-extensions
uv pip install git+https://github.com/openai/whisper.git
# Change depends on your device for inference.
uv pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
# for vscode jupyter
uv pip install ipykernel
```

## 3. Install `ffmpeg` and add to system environment variables
Download from https://ffmpeg.org/download.html
