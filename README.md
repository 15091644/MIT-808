# MIT-808
This repository handles the MIT 808 data science project.

Setting up:

1. After cloning the repository open anaconda prompt and naviagte to the local repo on your desktop
2. Create a virtual environment using conda using the following steps:
2.1. conda create -n MIT808 
2.2. Then once created: conda activate MIT808. You working with a separate controllable library environment in python.
2.3. conda install --yes --file requirements.txt to install the required dependencies
2.4 Separately install pytorch on conda using the following command depending on the GPU you have:

This is for windows:

CUDA available:

conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch

conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch

if CPU only:

conda install pytorch torchvision torchaudio cpuonly -c pytorch

Please see https://pytorch.org/ if you have another operating system.
