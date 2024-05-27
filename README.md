# S2L2-V2M

## Setting

We use Python 3.9.17 for this project and the library requirements are given in requirements.txt. Create a conda environment using
```
conda create --name <env> --file requirements.txt
```
Ensure that the NVIDIA Driver is version 12 or above to be compatible with PyTorch 2.1.0.

For the working of our model, Facebook's LLaMA-2 model weights are required, details on obtaining these weights are given on [HuggingFace](https://huggingface.co/docs/transformers/main/model_doc/llama). 

## Dataset

The dataset is available for download here:
- [MUVideo](https://huggingface.co/datasets/M2UGen/MUVideo)

## Model Training

To train the model, run the [**_train_musicgen.sh_**] script. 

## 🔨 Model Testing and Evaluation

To test the model, run [**_gradio_app.py_**].

For training, we use 4 24GB 4090 GPU. For inference, a single 24GB 4090 GPU is used.

## 🫡 Acknowledgements

This code contains elements from the following repo:
- [crypto-code/MU-LLaMA](https://github.com/crypto-code/MU-LLaMA)
- [M2UGen](https://github.com/shansongliu/M2UGen)
- [MA-LMM](https://github.com/boheumd/MA-LMM)
