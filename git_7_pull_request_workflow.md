# Submit Pull Request / Workflow

### Step 1:  fork the repo (on GitHub)
https://github.com/WiMLDS/python_advanced

### Step 2:  copy forked url for cloning 
* copy HTTPS url

### Step x:  go to working directory (your local terminal)
* go to whatever your working directory is
>my example
```bash
cd /Users/reshamashaikh/ds/gitsample
```

### Step x:  clone the repo  
<kbd> git clone <url> </kbd> 
>my example
```bash
git clone https://github.com/reshamas/python_advanced.git
```

### Step x:  `cd` into the repo
<kbd> cd <repo_name> </kbd>
>my example
```bash
cd python_advanced 
```

#### Step xb:  look at remotes
<kbd> git remote -v </kbd>
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
```

### Step x:  add remote
<kbd> git remote add upstream <url> </kbd>
>my example
```bash
git remote add upstream https://github.com/WiMLDS/python_advanced.git
```

#### Step xb:  look at remotes
<kbd> git remote -v </kbd>  
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
upstream	https://github.com/WiMLDS/python_advanced.git (fetch)
upstream	https://github.com/WiMLDS/python_advanced.git (push)
```

### Step 3:  update a repo
* copies changes from a remote repository to a local repository.
**Note:**  this is a good step to practice even though the first time you clone a repo it will already be up to date.   

<kbd> git pull </kbd> 

 
### Step 4:  create a working branch
<kbd> git branch <branch_name> </kbd>
>my example  
`git branch reshama_wip`

### Step 5:  switch to working branch
<kbd> git checkout <branch_name> </kbd>  
>my example  
`git checkout reshama_wip`

### Step 5:  create a file
* create a folder with your name here:  https://github.com/WiMLDS/python_advanced/tree/master/submissions
* `cd` into this folder, create a Python file with your name.  (Example:  `reshama.py`)

### Step 6:  add/stage a file
<kbd> git add <file_name> </kbd>  
>my example  
`git add reshama.py`

### Step 7:  commit a file
<kbd> `git commit -m 'message' </kbd>
>my example
 `git commit -m 'adding my python name file`
 
### Step 8:  push changes to your 'working branch'
<kbd> git push origin <branch_wip> </kbd>  
>my example
`git push origin reshama_wip`


### Step x:  submit pull request (on GitHub)

