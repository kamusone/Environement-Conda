# Environement-Conda


Software Installation

This is a technical class. You will need to be able to compile and execute Python code that makes use of TensorFlow for deep learning. There are two options to you for accomplish this:

    Install Python, TensorFlow and some IDE (Jupyter, TensorFlow, etc.)
    Use IBM Cognitive Class Labs online

Installing Python and TensorFlow

It is possible to install and run Python/TensorFlow entirely from your own computer. Google provides TensorFlow for Windows, Mac and Linux. Previously, TensorFlow did not support Windows. However, as of December 2016, TensorFlow supports Windows for both CPU and GPU operation.

The first step is to install Python 3.7. As of January 2019, this is the latest version of Python 3. I recommend using the Miniconda (Anaconda) release of Python, as it already includes many of the data science related packages that will be needed by this class. Anaconda directly supports: Windows, Mac and Linux. Miniconda is the minimal set of features from the very large Anaconda Python distribution. Download Miniconda from the following URL:

    Miniconda

Dealing with TensorFlow incompatibility with Python 3.7

*Note: I will remove this section once TensorFlow adds support for Python 3.7.

VERY IMPORTANT Once Miniconda has been downloaded you must create a Python 3.6 environment. TensorFlow does not currently (as of Jan 2019) support Python 3.7. So you must execute the following commands:

### conda create --name tensorflow python=3.6

To enter this environment, you must use the following command (for Windows), this command must be done every time you open a new Anaconda/Miniconda terminal window:

### activate tensorflow

For Mac, do this:

source activate tensorflow

Installing Jupyter

it is easy to install Jupyter notebooks with the following command:

### conda install jupyter

Once Jupyter is installed, it is started with the following command:

jupyter notebook

The following packages are needed for this course:

conda install scipy
### pip install --upgrade sklearn
### pip install --upgrade pandas
### pip install --upgrade pandas-datareader
### pip install --upgrade matplotlib
### pip install --upgrade pillow
### pip install --upgrade requests
### pip install --upgrade h5py
### pip install --upgrade pyyaml
### pip install --upgrade psutil
### pip install --upgrade tensorflow==1.12.0
### pip install --upgrade keras==2.2.4

Notice that I am installing as specific version of TensorFlow. As of the current semester, this is the latest version of TensorFlow. It is very likely that Google will upgrade this during this semester. The newer version may have some incompatibilities, so it is important that we start with this version and end with the same.

You should also link your new tensorflow environment to Jupyter so that you can choose it as a Kernal. Always make sure to run your Jupyter notebooks from your 3.6 kernel. This is demonstrated in the video.

python -m ipykernel install --user --name tensorflow --display-name "Python 3.6 (tensorflow)"

