# xgboost-fed-flower

This is a step by step tutorial for running xgboost with flower federated framework

first step is create a virtualenv using pyenv for running the framework, this to let you have a stable, reproducible, and portable environment. You are in control of which packages versions are installed and when they are upgraded.

**step 1:** install pyenv from this link : **https://github.com/pyenv-win/pyenv-win**
unzip the file from into a path called : **pyenv-win-master** </br>
</br>
**step 2:** Create a new folder .pyenv in your user folder with the name .pyenv. You can do this using the Explorer or the following PowerShell commands below
| Command | Description |
| --- | --- |
|mkdir $HOME/.pyenv | this is command to make local path for .pyenv in the users |
</br>
**step 3:** Extract the ZIP-archive and copy the pyenv-win folder and the .version file from the pyenv-win-master folder into the newly created .pyenv folder in your user folder.
</br>
| Command | Description |
| --- | --- |
|[System.Environment]::SetEnvironmentVariable('PYENV',$env:USERPROFILE + "\.pyenv\pyenv-win\","User")|| these are commands to set the environment variables PYENV and PYENV_HOME that point to the installation folder|
|[System.Environment]::SetEnvironmentVariable('PYENV_HOME',$env:USERPROFILE + "\.pyenv\pyenv-win\","User")|
