# GitStash

- Creates a up-to-date requirements file for python Venv
- Asks to add, commit and push

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

- http://thediscoblog.com/blog/2014/03/29/custom-git-commands-in-3-steps/
- https://coderwall.com/p/bt93ia/extend-git-with-custom-commands

- Don't put a file extension on the file when creating
- Include the git-stash file in the PATH
