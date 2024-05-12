# langchain

This is where I'll keep my different langchain tryouts

Setup had to change these
"notebook.output.wordWrap": true
"python.languageServer": "Pylance"

### Enabling GPU support in ollama
```
Get the UUID: nvidia-smi -L
nano /etc/systemd/system/ollama.service

CUDA_VISIBLE_DEVICES=GPU-e6819fdd-d3f9-1946-2c8f-415536bb5cfb

sudo systemctl daemon-reload
sudo systemctl restart ollama

nvidia-smi
```