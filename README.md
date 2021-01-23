# SHORTCUT
Custom command scripts to speed up development

1. Add C:\Program Files\Git\cmd to path ("enviromental variables")
2. Download Zip of this repo
3. Copy desired commands into C:\Program Files\Git\cmd
4. Execute by running ```git <cmd name>```

NOTE: Don't run from within an active venv (error, can't find file), script activates venv

## CMD > git new-python-prj

- Sets up a new python repository based on [PythonTemplate](https://github.com/marmstr93ng/PythonTemplate.git)

1. Create repository in github - No additional files
2. Navigate to desire local repository location
3. Run ```git new-python-prj <repo-name> <local-name (optional)>``` in the directory where the local copy is to be stored

## CMD > git exist-clone

- Clones a specified repo

1. Run ```git exist-clone <repo-name> <local-name (optional)>``` in the directory where the local copy is to be stored

## CMD > git exist-clone-python

- Clones a specified repo, setups up python virtual enviroment and installs packages specified in requirements.txt (runs ```git install-req```)

1. Run ```git exist-clone-python <repo-name> <local-name (optional)>``` in the directory where the local copy is to be stored

## CMD > git install-req

- Activate Venv, installs packages specified in requirements.txt

## CMD > git ship

- Asks to add, commit and push

## CMD > git ship-python

- Creates a up-to-date requirements file for python Venv
- Asks to add, commit and push

## CMD > git frigid

- Activate Venv, ***install package*** and update requirements.txt

## CMD > git warm

- Activate Venv, ***uninstall package*** and update requirements.txt

---

#### How-to Create a Git Command Aliase:
NOTE: Don't put a file extension on the file when creating

NOTE: ```source "$(git --exec-path)/git-sh-setup"``` only available in .git dir

[Sources]
1. http://thediscoblog.com/blog/2014/03/29/custom-git-commands-in-3-steps/
2. https://coderwall.com/p/bt93ia/extend-git-with-custom-commands
