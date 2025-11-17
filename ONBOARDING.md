# Onboarding Guide

## 1. SSH Access
Connect to the HPC system:
ssh ..t3

## 2. Create Workspace
Prepare a working directory:
mkdir -p ~/gpu_env
cd ~/gpu_env

## 3. Purge Modules
Clear all loaded environment modules:
module purge
module list

## 4. Verify Python
Check Python availability:
python3 --version

## 5. Create Virtual Environment
Make a clean Python venv:
python3 -m venv ~/llm_env

## 6. Activate Virtual Environment
Enable environment:
source ~/llm_env/bin/activate

## 7. Verify Environment Paths
Ensure venv is active:
which python
which pip
