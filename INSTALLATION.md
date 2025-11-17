# Installation Guide

## 1. Update Pip
Ensure latest pip version:
pip install --upgrade pip

## 2. Install CUDA PyTorch
Install GPU-enabled PyTorch:
pip install torch --index-url https://download.pytorch.org/whl/cu121

## 3. Verify GPU Access
Test CUDA availability:
python - << 'EOF'
import torch
print("Torch:", torch.__version__)
print("CUDA:", torch.version.cuda)
print("GPU:", torch.cuda.is_available())
EOF

## 4. Install Core ML Packages
Add HuggingFace and dependencies:
pip install transformers accelerate safetensors sentencepiece huggingface_hub

## 5. Prepare Working Folder
Create directory for scripts:
mkdir -p ~/gpu_env/scripts

## 6. Confirm Environment Isolation
Ensure no system path mixed:
which python
which pip
