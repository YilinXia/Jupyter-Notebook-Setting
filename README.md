# Jupyter-Notebook-Setting
Customize Jupyter Notebook and Improve your Programming Experience

## Kernels
[Github Kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)
, a place where people summarized all kernels you are able to add to your jupyter notebook
For daily use, like data analysis, machien learning or deep learning, Python, R and octave could be three main kernels for me to use

### Install Jupyter Notebook
* install Python on your computer ([Python 3.7](https://www.python.org/downloads/))
* install Jupyter Notebook
   * You can use anaconda to install jupyter notebook
   * Here we use ```pip``` to install jupyter
   ```
   python3 -m pip install --upgrade pip
   python3 -m pip install jupyter
   ```
* After installing Jupyter Notebook, you can execute jupyter notebook
```
Jupyter Notebook
```

* You can also change the default directory of the home page
   * Generate the config file and you can get the address where the file is
```
jupyter notebook --generate-config
```
   * Search for the notebook_dir and change the value of dir  (**attention: Please delete the # at the very beginning**)
```
c.NotebookApp.notebook_dir = u'C:/Users/Brillanting/Jupyter'
```
   * Restart the jupyter notebook and you can find the default directory has been changed

Before beginning 
### Install Octave
* install Octave on Mac
Since there is no install package for Mac OS,  [Homebrew](https://brew.sh/) could be a site for us.
   * Type the following code in Terminal
   ```
   /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”
   ```
   * Upgrade and update brew
   ```
   brew upgrade && brew update
   ```
  * Install octave wait for about 10 minutes
  ```
  brew install octave
  ```
  
* intsall Octave on Windows [Octave Download](https://www.gnu.org/software/octave/download.html)


* Install octave kernel
```
pip install octave-kernel
```


## Extensions
