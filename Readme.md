**How to set up Background-matting** 

# First step is to set up envirements and tools 

    tools that you need : 
    1- Git to clone repo 
    2- anaconda 

## Git 

You need to install Git from the following : 

 *  [Git link](https://git-scm.com/)
 
 Tip : if you're not familiar with Git commands , you just need to use github desktop to clone repos 

## Anaconda and Python 

 **I highly recommend to follow this [youtube video instructions](https://www.youtube.com/watch?v=5mDYijMfSzs&ab_channel=ProgrammingKnowledge)
 
 This is the most important step so you should follow instructions step by step 

 It is possible to install and run Python/Anaconda entirely from your computer, without the need for Google CoLab. Running Anaconda locally does require some software configuration and installation. If you are not confortable with software installation, just use Google CoLab. These instructions show you how to install Anaconda for both CPU and GPU.

 *Google Colab* pro is available as an option for 10$ per month 

 The first step is to install Python. I recommend using the Miniconda (Anaconda) release of Python. Anaconda directly supports Windows, Mac, and Linux. Miniconda is the minimal set of features from the extensive Anaconda Python distribution. Download Miniconda from the following URL:

 * [MiniConda](https://docs.conda.io/en/latest/miniconda.html)

 **Or just google miniconda and install it** 
 
 open anaconda terminal : 
 1. excute this line 
    ~~~~
    conda install -y jupyter
    ~~~~
 2.  Each environment that you create can have its own Python version, drivers, and Python libraries. I suggest that you create an environment to hold the Python instance for this class. Use the following command to create your environment. I am calling the environment Background, you can name yours whatever you like. 
    ~~~~
    conda create --name Background 
    ~~~~
 3. To enter this environment, you must use the following command:
    ~~~~
    conda activate Background
    ~~~~
 4. For now, lets add Jupyter support to your new environment.
    ~~~~
    conda install -c conda-forge nb_conda
    ~~~~
 
 5. Now we install pip managing package 
    ~~~~
    conda install -U pip 
    ~~~~
 6. Installing the following packages 
    ~~~~
    pip install kornia==0.4.1
    pip install tensorboard==2.3.0
    pip install torch==1.7.0
    pip install torchvision==0.8.1
    pip install tqdm==4.51.0
    pip install opencv-python==4.4.0.44
    pip install onnxruntime==1.6.0
    ~~~~

7. Register your Environment 
    The following command registers your Background environment. Again, make sure you "conda activate" your new Background environment.
    ~~~~
    python -m ipykernel install --user --name Background --display-name 
    ~~~~
8. Testing your Environment 
    You can now start Jupyter notebook. Use the following command.
    ~~~~
    jupyter notebook
    ~~~~

end  


