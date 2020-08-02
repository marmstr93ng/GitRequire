# SHORTCUT
Custom command scripts to speed up development

1. Add C:\Program Files\Git\cmd to path ("enviromental variables")
2. Download Zip of this repo
3. Copy desired commands into C:\Program Files\Git\cmd
4. Execute by running ```git <cmd name>```

## GitShip

- Creates a up-to-date requirements file for python Venv
- Asks to add, commit and push

NOTE: Don't run from within an active venv (error, can't find file), script activates venv

### Python Virtual Enviroment
- Generate a python requirements file which contains all the python libraries used in the project.
```
pip freeze > requirements.txt
```
- use virtual enviroments to create a specific python interpreter instance
```
pip install -r requirements.txt
```

However, if a new library has been included in the Virtual environment the requirements.txt will need to be updated. Remembering to do this manually could be problematic instead the requirements file should be updated and added to the commit if there is a change!

### How-to Create a Git Command Aliase:
NOTE: Don't put a file extension on the file when creating

[Sources]
1. http://thediscoblog.com/blog/2014/03/29/custom-git-commands-in-3-steps/
2. https://coderwall.com/p/bt93ia/extend-git-with-custom-commands


## To-Do
1. Add custom pip install cmd for venv (See Pip Warm)
2. Command to activate/deactivate with a single command (save cd down to scripts)
3. Write instructions on how to use - download, add to path

Currently not being maintained due to the use of VS Code [ease of use](https://code.visualstudio.com/docs/python/environments).

### (1)Pip Warm
* Keep requirements.txt up-to-date
* Pip freeze when installing or uninstalling packages
* Ignore pylint and other specific packages
[Ignore Packages](https://stackoverflow.com/questions/23640182/ignore-certain-packages-and-their-dependencies-with-pip-freeze)
