# SHORTCUT
Custom command scripts to speed up development

1. Add C:\Program Files\Git\cmd to path ("enviromental variables")
2. Download Zip of this repo
3. Copy desired commands into C:\Program Files\Git\cmd
4. Execute by running ```git <cmd name>```

NOTE: Don't run from within an active venv (error, can't find file), script activates venv

## CMD > Git Python-env

- Sets up a new python repository based on [PythonTemplate](https://github.com/marmstr93ng/PythonTemplate.git)

1. Create a blank github repo
2. Run ```git python-env <repo-name>``` in the directory where the local copy is to be stored

## CMD > Git setup-clone

- Clones a specified repo

1. Run ```git setup-clone <repo-name>``` in the directory where the local copy is to be stored

## CMD > Git setup-python-clone

- Clones a the specified repo, setups up python virtual enviroment and installs packages specified in requirements.txt (runs ```git install-req```

1. Run ```git setup-clone <repo-name>``` in the directory where the local copy is to be stored

## CMD > Git install-req

- Activate Venv, installs packages specified in requirements.txt

## CMD > Git Ship

- Creates a up-to-date requirements file for python Venv
- Asks to add, commit and push

## CMD > Git Frigid/Warm

- Activate Venv, install/uninstall package and update requirements.txt

---

#### How-to Create a Git Command Aliase:
NOTE: Don't put a file extension on the file when creating
NOTE: ```source "$(git --exec-path)/git-sh-setup"``` only available in .git dir

[Sources]
1. http://thediscoblog.com/blog/2014/03/29/custom-git-commands-in-3-steps/
2. https://coderwall.com/p/bt93ia/extend-git-with-custom-commands
