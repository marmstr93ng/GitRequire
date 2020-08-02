# SHORTCUT
Custom command scripts to speed up development

1. Add C:\Program Files\Git\cmd to path ("enviromental variables")
2. Download Zip of this repo
3. Copy desired commands into C:\Program Files\Git\cmd
4. Execute by running ```git <cmd name>```

## CMD > Git Ship

- Creates a up-to-date requirements file for python Venv
- Asks to add, commit and push

NOTE: Don't run from within an active venv (error, can't find file), script activates venv

## CMD > Git Python-env

- Sets up a new python repository based on [PythonTemplate](https://github.com/marmstr93ng/PythonTemplate.git)

1. Create a blank github repo
2. Run ```git python-env <repo-name>``` in the directory where the local copy is to be stored

## CMD > Git Frigid/Warm

- Activate Venv, install/uninstall package and update requirements.txt

---

# Info
#### Python Virtual Enviroment
- Generate a python requirements file which contains all the python libraries used in the project.
```
pip freeze > requirements.txt
```
- use virtual enviroments to create a specific python interpreter instance
```
pip install -r requirements.txt
```

[Github Package Source](https://stackoverflow.com/questions/16584552/how-to-state-in-requirements-txt-a-direct-github-source)

However, if a new library has been included in the Virtual environment the requirements.txt will need to be updated. Remembering to do this manually could be problematic instead the requirements file should be updated and added to the commit if there is a change!

#### How-to Create a Git Command Aliase:
NOTE: Don't put a file extension on the file when creating
NOTE: ```source "$(git --exec-path)/git-sh-setup"``` only available in .git dir

[Sources]
1. http://thediscoblog.com/blog/2014/03/29/custom-git-commands-in-3-steps/
2. https://coderwall.com/p/bt93ia/extend-git-with-custom-commands
