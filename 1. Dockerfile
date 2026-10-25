FROM pytorch/pytorch:2.1.2-cuda12.1-cudnn8-runtime
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y --no-install-recommends \
    ffmpeg xvfb python3-tk tk-dev libgl1-mesa-glx libglib2.0-0 sudo \
    && rm -rf /var/lib/apt/lists/*
RUN python3 -m pip install --upgrade pip
RUN pip install --no-cache-dir openai numpy opencv-python-headless pillow
WORKDIR /root
