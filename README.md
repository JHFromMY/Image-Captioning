# Image Captioning
An application that help generate caption for a list of selected travel images so that user can reduce caption creation effort when they post them in social media.

# 0_Setup
## Computer Selection
0. Make sure your purchased computer had support GPU and native window.

## Virtual Envitronment Setup
1. Install Anaconda (https://www.anaconda.com/download).
2. Open Ananconda Prompt to check CUDA and , 'nvidia-smi', else install from https://developer.nvidia.com/cuda-11-8-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local
3. Then, create an virtual environment, 'conda create -n ImageCaption python=3.10'
4. Then, activate the environment, 'conda activate ImageCaption'

## Kernel Setup
5. Then, move directory, 'cd C:\Users\User\Downloads\ImageCaption\0_Setup'
6. Then, install all dependency, 'pip install -r requirements.txt'
7. Then, install torch, 'pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118'
8. Then, create an external kernel, 'python -m ipykernel install --user --name=ImageCaption --display-name "ImageCaption"'
9. Download 'ImageCaption30K_InceptionV3_LSTM.ipynb' and loacte at 'C:\Users\User\Downloads\ImageCaption\2_Model\InceptionV3_LSTM'
10. Open Jupter Notebook and select "ImageCaption" kernel

In case need to add/update the external kernel:
1. Open Anancoda Prompt
2. Then, activate the environment, 'conda activate ImageCaption'
3. Then, add/modify using 'pip install' or 'pip uninstall'

In case need to remove the external kernel:
1. Open Anancoda Prompt
2. To remove kernel from Jupyter Notebook, 'jupyter kernelspec uninstall imagecaption'
3. For clean up, remove the entire folder, C:\Users\User\anaconda3\envs\ImageCaption

# 1_Data
1. Flickr30k dataset (https://www.kaggle.com/datasets/hsankesara/flickr-image-dataset) for medium-sized image captioning, IC30K.zip
2. GloVe: Global Vectors for Word Representation (https://nlp.stanford.edu/projects/glove/) for embedding purpose, 'glove.2024.wikigiga.300d.zip'

# 2_Model
## Data
