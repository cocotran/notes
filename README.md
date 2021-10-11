# Helpful Commands
List of helpful commands because I have bad memory

## Git
```bash
git diff --color-words    # instead of showing the line-by-line diff, it shows only the words that changed
```
```bash
git rm -r --cached [dir/file]
```
```bash
git push origin --delete [remoteBranchName]
```


## Local
```bash
sudo lsof -i :[portNumber]    # returns the user processes that are active on a port
sudo kill -9 PID              # kill the process
```

## JavaScript  
To update node.js
```bash
npm cache clean -f    # clear the npm cache
npm install -g n      # install Node’s version manager
sudo n stable         # or sudo n lastest or sudo n [version.number]
```


## Python

#### Pip
```bash
pip install [PACKAGE] && pip freeze | grep [PACKAGE] >> requirements.txt    # install and add specific package to requirement.txt
```

#### Flask
```bash
export FLASK_ENV=development    # set env to development
flask run
```

#### FastApi
```bash
uvicorn main:app --reload     
```

#### Cython
```bash
python3 setup.py build_ext --inplace  # build cython python
```
```bash
cython -a file.pyx              # generate HTML file
```



## Docker
```bash
sudo docker images   # list all images
```
```bash
sudo docker ps   # list all containers
```
```bash
sudo docker build -t [image-tag] [dir]   # build image and set name to image-tag
```
```bash
docker run -d -p [host-port]:[container-port] [image]
```
```bash
sudo stop {container]   # stop a container
```
