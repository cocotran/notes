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

---


## Node.js

#### Update Node.js
```bash
npm cache clean -f	# clear the npm cache
npm install -g n    # install Node’s version manager
sudo n stable       # or sudo n lastest or sudo n [version.number]
```