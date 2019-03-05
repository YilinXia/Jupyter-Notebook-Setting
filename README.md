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

## Extensions
Reference: https://www.jianshu.com/p/a85bc2a8fa56   / http://resuly.me/2017/11/03/jupyter-config-for-windows/
<br>Extension is another feature for jupyter notebook
* Change the theme
```
# install jupyterthemes
pip install jupyterthemes

# Set  Default theme
jt -r
```
* After the above operation, you can find the file in this directory
   * Windows C:/Users/username/.jupyter/custom
   * Mac: /Users/username/.jupyter/custom
* Here you can change the font or color or shortcut to revise certain code [Demo Someone Created](https://github.com/YilinXia/Jupyter-Notebook-Setting/blob/master/custom.zip)

* Install all extensions for jupyter
```
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user

pip install jupyter_nbextensions_configurator
jupyter nbextensions_configurator enable --user
```
* Enable extensions
```
jupyter nbextension enable collapsible_headings/main
jupyter nbextension enable code_prettify/code_prettify
```
**attention** the file followed ```enable``` is some ```JS```file <br>
**Mac** /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages/jupyter_contrib_nbextensions<br>
**Windows** C:\Users\username\AppData\Local\Programs\Python\Python37\Lib\site-packages\jupyter_contrib_nbextensions
