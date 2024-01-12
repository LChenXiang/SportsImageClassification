# Sports Non-Sports Classification model



## How to setup
Make sure [Anaconda](https://www.anaconda.com/download) is installed to continue. <br />
The .yaml environment file is tested on Windows based system, so Linux/Mac should follow another instruction below.

If you want to use the base environment and just add the extra packages:<br />
Navigate to the base folder of the project with the anaconda cmd, and enter:<br />

**conda env update -n base --file env.yaml**<br />

This should add packages on top of your current environment.<br />
<br />
If you want to create a new environment:<br />
Enter the following, after navigating to the project folder:<br />

**conda env create -f env.yaml <br />**

This should create a new anaconda environment named fyp.


## For Linux/Mac, or if the above doesn't work:
If you manage to try out the previous step without error, then feel free to ignore this.<br />
If not, after installing Anaconda, go to [PyTorch](https://pytorch.org/) website and select the appropriate commands required to install PyTorch
and paste it into the conda cmd prompt, either in the base env or in a new env if you choose to do so.
<br />
We are not adding any extra packages on top of Anaconda's given packages, aside from PyTorch, so by then you should be done.


## Starting the Flask Server
With the conda env selected and in the root directory (where app.py is located),
enter the following:<br />

**python -m flask run** 

to start the Flask server. If successful, the local IP to the website
should be displayed. Copy the link and open on your preferred browser.

Common Issues at this part:
- The term 'conda' is not recognized<br />
    This is because during installation of Anaconda, the PATH environment variable change option was not selected.
    To fix this, open up anaconda's cmd prompt, and type: conda init powershell
    Then try running the flask run command again.

