# VOICE_CLONING
## INSTALL REQUIREMENTS

## STEP 1:

Download and Install Anaconda (https://www.anaconda.com/)

## STEP 2:
Open Anaconda 3 CMD

## STEP 3:

Installing python 9.8

## STEP 4:

Create a new environment with Python 

`conda create --name voice-clone python
`
## STEP 5:

Activate the environment

`conda activate voice-clone`

## STEP 6: 
Install ffmeg (https://anaconda.org/conda-forge/ffmpeg)

`conda install -c conda-forge ffmpeg
`
## STEP 7:
Install PyTorch

 `conda install pytorch==1.10.1 torchvision==0.11.2 torchaudio==0.10.1 cpuonly -c pytorch` 

 (Install pytorch) – https://pytorch.org/get-started/previous-versions/

## STEP 8:
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

## STEP 11:
Toolbox with Dataset

`python demo_toolbox.py -d C:\Users\…
`

## TKINKTER USER INTERFACE PROGRAM 
`from tkinter import *
from tkinter import ttk, Label


def download():
    btndl = Label(window, text="start downloading...", bg="#1f376a", fg="white")
    btndl.pack()


window = Tk()
window.geometry("300x250")
window.title("VC")
window.config(bg="#1f376a")
window.iconbitmap("vc1.ico")

heading = Label(window, text="VOICE CLONE",bg="#1f376a", fg="white", font=("times", 10, "bold"),pady=10)
heading.grid(row=0, column=0)

tbname1 = Label(window, text="TEXT BOX", bg="#1f376a", fg="white",font=("times", 10, "bold"),pady=10)
tbname1.grid(row=1, column=0)
textbox = Entry(window, width=30, font=("times", 10), bg="#DBC2AD")
textbox.grid(row=1, column=3)

tbname2 = Label(window, text="VOICES",bg="#1f376a", fg="white", font=("times", 10, "bold"),pady=20)
tbname2.grid(row=2, column=0)
checkbox = ttk.Combobox(window, width=26, state="readonly")
checkbox['values'] = ("Regan", "Leena", "Ranjith", "Pilavendran")
checkbox.grid(row=2, column=3)

clone = Button(window, text="CLONE", bg="grey", fg="white", padx=30, pady=7, width=6, activebackground="#a0a0a0",
              activeforeground="black", command=download )
clone.grid(columnspan=5,rowspan=3)


dowl = Button(window, text="Download", bg="grey", fg="white", padx=30, pady=7, width=6, activebackground="#a0a0a0",
              activeforeground="black", command=download)
dowl.grid(columnspan=5,rowspan=3)

window.mainloop()`
