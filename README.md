# VOICE_CLONING
#INSTALL REQUIREMENTS

##STEP 1:

Download and Install Anaconda (https://www.anaconda.com/)

##STEP 2:
Open Anaconda 3 CMD

##STEP 3:

Installing python 9.8

##STEP 4:

Create a new environment with Python 

`conda create --name voice-clone python
`
##STEP 5:

Activate the environment

`conda activate voice-clone`

## STEP 6: 
Install ffmeg (https://anaconda.org/conda-forge/ffmpeg)

`conda install -c conda-forge ffmpeg
`
##STEP 7:
Install PyTorch

 `conda install pytorch==1.10.1 torchvision==0.11.2 torchaudio==0.10.1 cpuonly -c pytorch` 

 (Install pytorch) – https://pytorch.org/get-started/previous-versions/

##STEP 8:
Install additional requirements

`pip install Unidecode`

`pip install inflect`

`pip install sounddevice`

`pip install umap`

`pip install PyQt5`

`pip install webrtcvad-wheels`

`pip install webrtcvad`


## STEP 9:
Run the demo

`python demo_toolbox.py`

## STEP 10:
Launch the Toolbox

`python demo_toolbox.py `(without data)

##STEP 11:
Toolbox with Dataset

`python demo_toolbox.py -d C:\Users\…
`
