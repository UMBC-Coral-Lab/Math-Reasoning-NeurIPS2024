

# SBI-RAG

This repository is the official implementation of [SBI-RAG: Enhancing Math Word Problem Solving for Students through Schema-Based Instruction and Retrieval-Augmented Generation](https://arxiv.org/abs/2410.13293). 

<h2>SBI-RAG Architecture</h2>
<img src="Assets/SBI_RAG.jpg" alt="SBI-RAG Architecture">

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

>📋  Describe how to set up the environment, e.g. pip/conda/docker commands, download datasets, etc...

## Training

>📋 To train your Schema classifier model access the "Schema Classifier trained on a custom Schema Based Dataset" part in the colab notebook, you can try different hyperparameter according to your choice. 



## Pre-trained Models

You can download pre-trained schema models here:

- [Pre-Trained Schema Classifier Models](https://drive.google.com/drive/folders/1DnT32TGP4XAMuR1AHVeEkO0e3nMg_KmI?usp=sharing) trained on DistilBert using parameters in the training arguments. 

>📋  Give a link to where/how the pretrained models can be downloaded and how they were trained (if applicable).  Alternatively you can have an additional column in your results table with a link to the models.

## Results

Our model achieves the following performance on :

### [Image Classification on ImageNet](https://paperswithcode.com/sota/image-classification-on-imagenet)

| Model name         | Top 1 Accuracy  | Top 5 Accuracy |
| ------------------ |---------------- | -------------- |
| My awesome model   |     85%         |      95%       |

>📋  Include a table of results from your paper, and link back to the leaderboard for clarity and context. If your main result is a figure, include that figure and link to the command or notebook to reproduce it. 


## Contributing

>📋  Pick a licence and describe how to contribute to your code repository. 
