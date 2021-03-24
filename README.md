# Jupyter-Kernel-Settings
Customize Jupyter Notebook and Improve Programming Experience

## Conda Environment
create a conda env and install jupyter python

### Set Octave Kernel
ref:https://github.com/calysto/octave_kernel


## Local Environment
[Github Kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)
, a place where people summarized all kernels you can add to your jupyter notebook for daily use, like data analysis, machine learning, or deep learning. Python, R, and Octave are the pervasive kernels.

### Install Jupyter Notebook
* install Python on your computer
* install Jupyter Notebook
* After installing Jupyter Notebook, you can execute jupyter notebook
```
Jupyter Notebook
```
* You can also change the default directory of the home page
by generating the config file, and you can get the address where the file is
```
jupyter notebook --generate-config
```
   * Search for the notebook_dir and change the value of dir  (**attention: Please delete the # at the very beginning**)
```
c.NotebookApp.notebook_dir = u'C:/Users/Brillanting/Jupyter'
```
   * Restart the jupyter notebook, and you will find the default directory has been changed

## Install Kernels
most kernels based on the existing software in your computer <br>

### Install Octave
**macOS**

* install Octave on Mac
   
Since there is no install package for Mac OS,  we will use [Homebrew](https://brew.sh/) to install it

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”`
      
* Probably it will ask you to upgrade and update brew

`brew upgrade && brew update`

* Install octave wait for about 10 minutes
`brew install octave`

* Install octave kernel
`pip install octave-kernel`

**Windows**
* install Octave on Windows [Octave Download](https://www.gnu.org/software/octave/download.html)

* Add environment path
```
Variable Name: OCTAVE_EXECUTABLE
Variable Value: E:\Octave\Octave-5.1.0.0\mingw64\bin\octave-cli.exe
```

* Change the tornado to 5.1.1
`pip3 install tornado==5.1.1`

* Install octave kernel
`pip install octave-kernel`

### Install R
Reference: IRkernel [Github Instruction](https://github.com/IRkernel/IRkernel)

Type command in R
```
install.packages('IRkernel')
IRkernel::installspec()  # to register the kernel in the current R installation
```
Then 
```
IRkernel::installspec(name = 'ir33', displayname = 'R 3.3')
```
