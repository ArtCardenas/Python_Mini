# Python_Mini

## Python Version
```powershell
python --version     # Windows
python3 --version    # Linux
sudo apt-get update  # Linux
```

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
virtualenv --python $(which python) ~/artvenv

# activate virtual environment Windows
artvenv\Scripts\activate
# alternate Linux
source ~/artvenv/bin/activate


# install packages
python -m pip install numpy
python -m pip install scikit-learn
```
```bash
# deactivate
deactivate

# upgrade pip
python.exe -m pip install --upgrade pip
python -m pip list
python3 -m pip list
```

## Notes from Noah Gift
====================================================
Compiling Python from scratch with Github Codespaces
https://www.youtube.com/watch?v=gzh329Yzv8E
https://github.com/nogibjj/compile-python

`sudo apt-get install build-essential gdb lcov libbz2-dev libffi-dev libgdbm-dev liblzma-dev libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev lzma lzma-dev tk-dev uuid-dev zlib1g-dev`

htop

./configure --enable-optimizations

# use 16 cpus for python
make -j 16
sudo make altinstall
/usr/local/bin/python3.10

========================
vim ~/.bashrc
nano ~/.bashrc
# add new python inside .bashrc
alias python="/usr/local/bin/python3.10"
# source venv
source ~/.venv/bin/activate
========================
# from editor requirements.txt
<f1> python: create environment


# execute the file
source ~/.bashrc
which python


vim .gitignore
touch requirements.txt
touch Makefile
make install


