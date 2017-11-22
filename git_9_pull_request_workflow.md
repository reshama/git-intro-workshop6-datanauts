# Submit Pull Request / Workflow

### Step 1:  fork the repo (on GitHub)
https://github.com/WiMLDS/python_advanced

### Step 2:  copy forked url for cloning 
Click on the green button for your forked GitHub repo, and ensure it is showing the url for "Clone with HTTPS"  (other option is "Clone with SSH").  Copy that URL.    

<img src="images/github_clone_button.png" align="left" height="40" width="180" >


<img src="images/github_clone_button.png" alt="Drawing"  style="width: 100px;" style="height: 100px"/> 

<img src="images/chrome_curlwget.png" alt="Drawing" style="width: 100px;" style="height: 100px"/>  


>my example  
```text
https://github.com/reshamas/python_advanced.git
```

### Step 3:  go to working directory (your local terminal)
* go to whatever your working directory is
>my example
```bash
cd /Users/reshamashaikh/ds/gitsample
```

### Step 4:  clone the repo  
<kbd> git clone <url> </kbd> 
>my example
```bash
git clone https://github.com/reshamas/python_advanced.git
```

### Step 4:  `cd` into the repo
<kbd> cd <repo_name> </kbd>
>my example
```bash
cd python_advanced 
```

#### Step 5:  look at remotes
<kbd> git remote -v </kbd>
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
```

### Step 6:  add 'upstream' remote
<kbd> git remote add upstream <url> </kbd>
>my example
```bash
git remote add upstream https://github.com/WiMLDS/python_advanced.git
```

#### Step 7:  look at remotes
<kbd> git remote -v </kbd>  
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
upstream	https://github.com/WiMLDS/python_advanced.git (fetch)
upstream	https://github.com/WiMLDS/python_advanced.git (push)
```

### Step 8:  update a repo
* copies changes from a remote repository to a local repository.
**Note:**  this is a good step to practice even though the first time you clone a repo it will already be up to date.   

<kbd> git pull </kbd> 

 
### Step 9:  create a working branch
<kbd> git branch <branch_name> </kbd>
>my example  
`git branch reshama_wip`

### Step 10:  switch to working branch
<kbd> git checkout <branch_name> </kbd>  
>my example  
`git checkout reshama_wip`

### Step 11:  create a file
* create a folder with your name here:  https://github.com/WiMLDS/python_advanced/tree/master/submissions
* `cd` into this folder, create a Python file with your name.  (Example:  `reshama.py`)

### Step 12:  add/stage a file
<kbd> git add <file_name> </kbd>  
>my example  
`git add reshama.py`

### Step 13:  commit a file
<kbd> git commit -m 'message' </kbd>
>my example
 `git commit -m 'adding my python name file`
 
### Step 14:  push changes to your 'working branch'
<kbd> git push origin <branch_wip> </kbd>  
>my example
`git push origin reshama_wip`


### Step 15:  submit pull request (on GitHub)

