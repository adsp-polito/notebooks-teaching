# notebooks-teaching

A collection of educational Jupyter notebooks demonstrating neural foundation models, Large Language Models (LLMs), fine-tuning, and transfer learning with benchmark datasets.

## Overview

This repository contains hands-on tutorials for working with state-of-the-art deep learning models and techniques. Each notebook is self-contained and includes detailed explanations, code examples, and visualizations.

## Notebooks

### 1. Vision Transformer with CIFAR-10 (`01_vision_transformer_cifar10.ipynb`)

Learn how to use a pre-trained Vision Transformer (ViT) foundation model for image classification.

**Topics Covered:**
- What are foundation models?
- Loading pre-trained Vision Transformer from Hugging Face
- Using CIFAR-10 benchmark dataset
- Zero-shot prediction capabilities
- Model evaluation and visualization

**Key Models:** Vision Transformer (ViT)  
**Datasets:** CIFAR-10

### 2. LLM Text Generation and Analysis (`02_llm_text_generation_imdb.ipynb`)

Explore Large Language Models for text generation and sentiment analysis.

**Topics Covered:**
- Introduction to Large Language Models (LLMs)
- Text generation with GPT-2
- Sentiment analysis with pre-trained BERT
- Working with IMDB benchmark dataset
- Comparing different LLM capabilities

**Key Models:** GPT-2, DistilBERT  
**Datasets:** IMDB Movie Reviews

### 3. Fine-tuning BERT for Sentiment Analysis (`03_finetuning_bert_sentiment.ipynb`)

Step-by-step guide to fine-tuning a pre-trained BERT model for a specific task.

**Topics Covered:**
- What is fine-tuning and why it's important
- Preparing data for fine-tuning
- Training loop and optimization
- Evaluation and metrics
- Saving and loading fine-tuned models
- Comparing pre-trained vs fine-tuned performance

**Key Models:** BERT  
**Datasets:** IMDB Movie Reviews

### 4. Transfer Learning for Image Classification (`04_transfer_learning_image_classification.ipynb`)

Comprehensive tutorial on transfer learning using ResNet for image classification.

**Topics Covered:**
- Transfer learning concepts and strategies
- Feature extraction approach (freeze all layers)
- Fine-tuning approach (unfreeze some layers)
- Comparing different transfer learning strategies
- Data augmentation techniques
- Model evaluation and visualization

**Key Models:** ResNet-18  
**Datasets:** CIFAR-10

## Installation

### Prerequisites
- Python 3.8 or higher
- CUDA-capable GPU (optional but recommended)

### Setup

1. Clone the repository:
```bash
git clone https://github.com/adsp-polito/notebooks-teaching.git
cd notebooks-teaching
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter:
```bash
jupyter notebook
```

4. Navigate to the `notebooks/` directory and open any notebook.

## Requirements

The main dependencies include:
- PyTorch >= 2.0.0
- Transformers >= 4.30.0
- Datasets >= 2.14.0
- TorchVision >= 0.15.0
- Jupyter
- NumPy, Pandas, Matplotlib, Seaborn
- scikit-learn

See `requirements.txt` for the complete list.

## Usage

Each notebook is designed to be self-contained and can be run independently. The notebooks will automatically download required datasets and models on first run.

**Note:** Some notebooks may require significant computational resources (GPU recommended) and storage for downloading models and datasets.

## Learning Path

We recommend following the notebooks in order:

1. Start with **Notebook 1** to understand foundation models with Vision Transformers
2. Move to **Notebook 2** to explore LLMs and their capabilities
3. Learn fine-tuning techniques in **Notebook 3**
4. Master transfer learning strategies in **Notebook 4**

## Key Concepts

### Foundation Models
Large-scale pre-trained models that can be adapted to various downstream tasks. Examples include Vision Transformers, BERT, and GPT.

### Fine-tuning
The process of taking a pre-trained model and further training it on a specific task or dataset, adapting the learned representations to your needs.

### Transfer Learning
Leveraging knowledge from models trained on one task to improve performance on a different but related task, often with less data and training time.

### Benchmark Datasets
Standardized datasets used to evaluate and compare model performance:
- **CIFAR-10:** 60,000 32x32 color images in 10 classes
- **IMDB:** 50,000 movie reviews for sentiment analysis

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the notebooks.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Hugging Face Transformers library
- PyTorch team
- CIFAR-10 and IMDB dataset creators
- Open-source ML community

## Citation

If you use these notebooks in your research or teaching, please cite:
```
@misc{notebooks-teaching,
  title={Educational Notebooks on Neural Foundation Models and Transfer Learning},
  author={ADSP Polito},
  year={2024},
  publisher={GitHub},
  url={https://github.com/adsp-polito/notebooks-teaching}
}
```