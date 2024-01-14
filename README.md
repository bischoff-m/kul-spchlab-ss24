# spchlab

*spchlab* is a Repository of Jupyter Noteboobs for Speech Recognition Demos and Exercises.

*spchlab* contains a number of different topics that are organized by folder (labxx_name).  Each of these is rather independent from each other, but knowledge and skills may be reuquired from lower numbered lab sessions.    

Each lab-folder contains:
- a README.md file with a general description of the folder contents.  It also describes which notebooks are rather tutorial in nature and which ones contain primarily exercises.
- a number of tutorials; they typically appear both in notebook tut_name.ipynb and in HTML tut_name.html format
- a number of exercises in notebook ExName.ipynb format

*spchlab* resides on GitHub and heavily relies on the *pyspch* package.   

## pyspch

*pyspch* is our own speech processing and recognition package that has grown over the years with spchlab.  It is not intended to be a full blown state of the art package to do speech recognition with.   Its focus is tutorial in nature and being a support package for spchlab.
* Packages that pyspch relies on:
  + *numpy, pandas, scipy, sklearn* as elementary packages supporting machine learning
  + *matplotlib, seaborn* for plotting 
  + *Pytorch, torchaudio, tensorflow*: for the exercises using DNNs



## Platforms and Requirements

The notebooks have been developed and tested on *Google Colab*, *Windows 10/11* and *MacOS*.
Generally speaking we expect the code to run on platforms supporting Python 3.9 or higher.  *pyspch* has a list of dependencies that guarantee (within the bounds of our testing) full functionality.  We also provide an .yml environment.
Generally we avoid features - from any package - that are considered very novel and tried to avoid future deprecation warnings.

So while the code is expected to be 99% platform independent, some dependencies are not:
- anything relating to AUDIO I/O tends to be hardware and platform dependent
- Some notebooks rely on pytorch and torch audio and have been tested in a CUDA environmnet;  CUDA is not available on MAC and the CPU-only version was not reliably tested


## Running a notebook in Google Colab

All of the notebooks can be run in [Google Colab](https://colab.research.google.com/).
There is no need to install software locally.  All you need is a browser to get access.  For most people Google Colab will be the easiest way to run the exercises provided in spchlab.  
To be able to use Google Colab, you need to have a Google account. If you have one, make sure you are logged in.

To run a notebook in COLAB:
  - go to the spchlab repository on Github [https://github.com/compi1234/spchlab]
  - click to open <notebook>.ipynb
  - now, do one of the following:
	1. click on the "open in colab" browser extension icon  (if you have it installed)
	2. Paste the GitHub exercise URL in a running colab session
  - start running the notebook in colab
  - neglect the Colab Warnings (see below)

### Colab WARNINGS
There are 2 innocent warnings that you will probably run into
1. After you install the pyspch package (which is almost always the first thing you need to do), you probably get a warning that you need to **restart the runtime**, Just CLICK and CONTINUE.
2. When you start running the notebook, you may get a warning that the notebook is not authored by Google.  Just ignore and click  'Run anyway'.

## Running the notebooks on your own PC

If you want to run these notebooks outside the Google Colab environment, e.g. on your own PC,  make sure to install the **pyspch** package (available in github/compi1234/pyspch).  

Dependencies:
+ preferably Python >=3.8, <=3.10
+ Most secure is to build a dedicated environment based e.g. on the available in py39.yml 
+ You may just add pyspch to your current environment, but be aware that this may lead to conflicts
+ Some notebooks require pytorch
    - look at https://pytorch.org/get-started/locally/  for installation instructions for pytorch and its dependencies



## Structure of our Jupyter notebooks
Jupyter notebooks contain a combination of text and Python code.  Notebooks are organized in cells. Text cells just contain an explanation of what is going on. Code cells can be executed one at a time by clicking on the arrow pointing to the cell. This step-by-step execution let's you follow at your own pace what is going on in a long and complex program. Strictly speaking there is no requirement that you execute cells from top to bottom, but in practice notebooks are often organized as such.  Especially the first couple of cells with imports and new function definitions should be run in their natural order.

## What do you need to know about Python ?
Our notebooks contain Python code. Most of the code (with the explanation) will be self-explanatory. You are not expected to write your own Python scripts or code (unless you do a project).  But you are expected from time to time to make small changes to parameters/ code flow ...

If you're not familiar with Python, following information may be worthwhile:
+ Python uses indexing starting at 0
+ Python is object oriented
+ The import statement defines packages and parts thereof for you current program, those cells are obviously essential


