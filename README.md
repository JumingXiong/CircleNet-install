# CircleNet-Installation

##choose your cuda version
Please refer this [Website]([https://www.google.com](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/)https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/) to see which cuda version you can choose.

## Operating System
[Optional but recommended] Ubuntu-20.04 or Ubuntu-18.04.
If you are using the Windows System, the best way to use Linux system is [Install Linux on Windows with WSL](https://learn.microsoft.com/en-us/windows/wsl/install)
For example to use Ubuntu18.04

## Install gcc and g++
update apt 
~~~
sudo apt update
~~~
install gcc and g++
~~~
sudo apt install gcc g++
~~~

## Anaconda/Miniconda 
Download Miniconda
~~~
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
~~~
Install Miniconda
~~~
sh Miniconda3-latest-Linux-x86_64.sh
~~~
restart terminal session
~~~
source .bashrc
~~~

## Setup virtual environment
Recommend python version 3.7 or 3.6,  pytorch version > 1.7
for example:
~~~
conda create -n CircleNet python=3.7
~~~
activate the environment
~~~
conda activate CircleNet
~~~
install Pytorch 1.11 and cudatoolkit 11.3
~~~
conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch
~~~

## Install Packages
1.  install Cython and pycocotools
~~~
pip install cython pycocotools
~~~
2.  clone this repo
~~~
git clone https://github.com/hrlblab/CircleNet.git
~~~
3.  install requirements
~~~
cd CircleNet
pip install -r requirements.txt
~~~



