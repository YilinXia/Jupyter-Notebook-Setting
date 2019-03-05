# Jupyter-Notebook-Setting
Customize Jupyter Notebook and Improve your Programming Experience

## Kernels
[Github Kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)
, a place where people summarized all kernels you are able to add to your jupyter notebook for daily use, like data analysis, machine learning or deep learning. Python, R and Octave could be three main kernels for me to use.

### Install Jupyter Notebook
* install Python on your computer ([Python 3.7](https://www.python.org/downloads/))
* install Jupyter Notebook
   * You can use anaconda to install jupyter notebook
   * Here I use ```pip``` to install jupyter<br><br>
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

Before installing other kernels, I'd like to say that most kernels are based on the existed softwares in your computer, so the first step usually is to install correpsonding software in your computer.<br>

### Install Octave
* Mac
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
   * Install octave kernel
   ```
   pip install octave-kernel
   ```
* Windows
   * intsall Octave on Windows [Octave Download](https://www.gnu.org/software/octave/download.html)

   * Add environment path
   ```
   Variable Name: OCTAVE_EXECUTABLE
   Variable Value: E:\Octave\Octave-5.1.0.0\mingw64\bin\octave-cli.exe
   ```
   * Change the tornado to 5.1.1
   ```
   pip3 install tornado==5.1.1
   ```
   * Install octave kernel
   ```
   pip install octave-kernel
   ```

### Install R


## Extensions
