# Image Captioning
An application that help generate caption for a list of selected travel images so that user can reduce caption creation effort when they post them in social media.

# 0_Setup
## Computer Selection
Make sure your purchased computer had support GPU and native Window.

## Resources
1. Install this github repository in your local device.
2. Make sure to change file structure as such:

. 
├── Downloads/
|    ├──ImageCaption/
|        ├──0_Setup/
|        └──1_Data/
|            └──glove.2024.wikigiga.300d.zip/
|                └──wiki_giga_2024_300_MFT20_vectors_seed_2024_alpha_0.75_eta_0.05_combined.txt
|            └──IC30K.zip/
|                └──flickr30k_images/
|                    └──flickr30k_images/
|                        └──....jpg
|                    results.csv
|        └──2_Model

## Virtual Envitronment Setup
1. Install Anaconda (https://www.anaconda.com/download).
2. Open Ananconda Prompt to check CUDA and , 'nvidia-smi', else install from https://developer.nvidia.com/cuda-11-8-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local
3. Then, create an virtual environment, 'conda create -n ImageCaption python=3.10'
4. Then, activate the environment, 'conda activate ImageCaption'

## Kernel Setup
1. Then, install all dependency, 'pip install -r C:/Users/User/Downloads/ImageCaption/0_Setup/requirements.txt'
2. Then, create an external kernel, 'python -m ipykernel install --user --name=ImageCaption --display-name "ImageCaption"'
3. Download 'ImageCaption30K_LSTM.ipynb' and loacte at 'C:\Users\User\Downloads\ImageCaption\2_Model\LSTM'
4. Open Jupter Notebook and select "ImageCaption" kernel

In case need to add/update the external kernel:
1. Open Anancoda Prompt
2. Then, activate the environment, 'conda activate ImageCaption'
3. Then, add/modify using 'pip install' or 'pip uninstall'
4. Restart kernel in Jupyter Notebook

In case need to remove the external kernel:
1. Open Anancoda Prompt
2. To check available kernel to delete, 'jupyter kernelspec list'
3. To remove kernel from Jupyter Notebook, 'jupyter kernelspec uninstall imagecaption'
4. For clean up, remove the entire folder, C:\Users\User\anaconda3\envs\ImageCaption

# 1_Data
1. Flickr30k dataset (https://www.kaggle.com/datasets/hsankesara/flickr-image-dataset) for medium-sized image captioning
2. GloVe: Global Vectors for Word Representation (https://nlp.stanford.edu/projects/glove/) for LSTM embedding purpose

# 2_Model
## Data
