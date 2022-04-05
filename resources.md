## Bash

#### Kill running process
```bash
sudo lsof -i :[portNumber]    # returns the user processes that are active on a port
sudo kill -9 PID              # kill the process
```

---

## Git

#### Show Git diff
```bash
git diff --color-words    # instead of showing the line-by-line diff, it shows only the words that changed
````

#### Delete file/folder from remote repository
```bash
git rm -r --cached [dir/file]
git push origin --delete [remoteBranchName]
```

#### Git config
```bash
git config --list         # show configuration
git config [key] "value"  # general syntax

git config user.name "cocotran"           # set repository-specific Git user name
git config --global user.name "cocotran"  # set global Git username
```

---

## Node.js

#### Update Node.js
```bash
npm cache clean -f	# clear the npm cache
npm install -g n    # install Node’s version manager
sudo n stable       # or sudo n lastest or sudo n [version.number]
```