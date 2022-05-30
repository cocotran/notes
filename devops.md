## Bash

#### Open ssh conenction
```bash
ssh user@hostname
```

#### Download file
```bash
wget <options> <url>
```

#### Install/uninstall rpm file
```bash
sudo rpm -i filename.rpm
sudo yum install filename.rpm

yum list installed [package_name] # find out whether a package is installed

rpm -e [package_name].noarch
```

####  Display a list of rpm packages installed
```bash
rpm -qa
```

#### Search for directory
```bash
find /path/to/search -type d -name "name-of-directory"
```
The -d option is what causes find to display directories (or folders) only. The -f option can be used for files, or the options can be omitted entirely to find both directories and files with the specified name.

#### Ping a port
```bash
telnet <host> <port>
Test-NetConnection <address> -p <port_number> # PowerShell
```

#### Kill running process
```bash
sudo lsof -i :[portNumber]    # returns the user processes that are active on a port
sudo kill -9 PID              # kill the process
```


---


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


---


## Git

#### Git squash
```bash
git reset --soft <commit>
git commit -m "new commit"
git push -f
````

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