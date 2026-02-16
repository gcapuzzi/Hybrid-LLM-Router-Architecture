# Hyperledger Fabric Expert SLM

This repository contains the resources for a comparison between a specialized Small Language Model (SLM) focused on Hyperledger Fabric (the model is a fine-tuned version of Qwen 2.5 7B Instruct) and an Agentic RAG architecture.

## Project Overview
The goal of this project is to demonstrate the effectiveness of vertical fine-tuning on technical domains using limited computational resources. The model has been optimized to provide accurate architectural and operational guidance for Hyperledger Fabric environments.

## Repository Contents
- qwen_training_data.json: The curated dataset used for Supervised Fine-Tuning (SFT), containing 200 technical instruction-output pairs.
- Qwen_Fabric_Expert_Demo.ipynb: Google Colab notebook to run the inference UI using Gradio and 4-bit quantization.
- agentic_rag_colab.ipynb: Google Colab notebook to evaluate Agentic RAG costs.

## Model Details
- Base Model: Qwen/Qwen2.5-7B-Instruct
- Fine-tuning Method: LoRA (Low-Rank Adaptation)
- Domain: Hyperledger Fabric (Architecture, Chaincode Lifecycle, Network Configuration)

## Hardware Requirements
To run the provided notebook, a GPU with at least 16GB of VRAM (such as NVIDIA T4 or L4) is required. The model is loaded in 4-bit precision to optimize memory usage (for Fine-Tuned SLM) while CPU for Agentic RAG.

## License
This project is licensed under the Apache License 2.0.
