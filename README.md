# xgboost-fed-flower

## This is a step by step tutorial for running xgboost with flower federated framework

first step is create a virtualenv using pyenv for running the framework, this to let you have a stable, reproducible, and portable environment. You are in control of which packages versions are installed and when they are upgraded.

**1:** install pyenv from this link : **https://github.com/pyenv-win/pyenv-win**
      unzip the file from into a path called : **pyenv-win-master** </br>
</br>
**2:** Create a new folder .pyenv in your user folder with the name .pyenv. You can do this 
       using the Explorer or the following PowerShell commands below

| Command | Description |
| --- | --- |
|mkdir $HOME/.pyenv|this is command to make local path for .pyenv in the users|

**3:** Extract the ZIP-archive and copy the pyenv-win folder and the .version file from the 
       pyenv-win-master folder into the newly created .pyenv folder in your user folder.
</br>
**4.** Run these commands to set the environment variables PYENV and PYENV_HOME that point to 
       the installation folder.
```console
[System.Environment]::SetEnvironmentVariable('PYENV',$env:USERPROFILE + "\.pyenv\pyenv-win\","User")
```
```console
[System.Environment]::SetEnvironmentVariable('PYENV_HOME',$env:USERPROFILE + "\.pyenv\pyenv-win\","User")
```
**5.** Add the bin folder to the PATH variable. Such that pyenv can be found when using the command line.
```console
[System.Environment]::SetEnvironmentVariable('path', $env:USERPROFILE + "\.pyenv\pyenv-win\bin;" + $env:USERPROFILE + "\.pyenv\pyenv-win\shims;" + [System.Environment]::GetEnvironmentVariable('path', "User"),"User")
```
**6.** Close the current PowerShell.If you haven’t enabled script execution yet, start a new PowerShell with admin privileges by right-clicking on the PowerShell icon in the start menu and choose Run as administrator.
![image](https://github.com/Astroherodvaipayan/xgboost-fed-flower/assets/105009701/e80145e9-3121-4aa5-bec4-165a6dd6f9ed)

```console
 Set-ExecutionPolicy unrestricted
```
