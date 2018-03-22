# git-practice
test using git

## Step
### 1.create master.js to master branch
```bash
$ git branch 
$ git status
$ nano master.js
$ git add master.js
$ git commit -m "add master.js to master branch"
$ git status
$ git push
```
Result
```bash
# READEME.md
# master.js
```

### 2.create slave.js to slave branch
```bash
$ git checkout -b "slave"
$ git status
$ nano slave.js
$ git add slave.js
$ git commit -m "add slave.js to slave branch"
$ git status
$ git push -u origin slave
```
Result
```bash
# README.md
# master.js
# slave.js
```

### 3.pull slave to master
```bash
$ git checkout master
$ git status
# READEME.md
# master.js
$ git pull origin slave
$ git status
# READEME.md
# master.js
# slave.js
$ git push
```
Result
```bash
# READEME.md (update from slave)
# master.js
# slave.js (update from slave)
```