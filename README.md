# Python_Mini

## Git
`git` commands

```bash
git status
git add main.py
git commit -m "pushing a build trigger 2nd time"

```

to push back to GitHub Repository, either normal or -f = Force
```bash
git push
git push -f 
```

to read from GitHub Repository to CodeSpace, either normal or -f = Force
```bash
git pull
git pull -f
```

## Python Environment
You can [follow instructions here](https://realpython.com/python-virtual-environments-a-primer/).

```bash
# create virtual environment
python -m venv artvenv
# alternative method, the ~/.    could be as just ~/artvenv
virtualenv --python $(which python) ~/.artvenv

# activate virtual environment Windows
artvenv\Scripts\activate
# alternate Linux
source ~/.artvenv/bin/activate


# install packages
python -m pip install numpy
```
```bash
# deactivate
deactivate

# upgrade pip
python.exe -m pip install --upgrade pip
python -m pip list
python3 -m pip list
```
