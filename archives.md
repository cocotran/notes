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
