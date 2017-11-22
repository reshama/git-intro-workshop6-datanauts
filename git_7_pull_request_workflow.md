# Submit Pull Request / Workflow

### Step 1:  fork the repo (on GitHub)
https://github.com/WiMLDS/python_advanced

### Step 2:  clone the repo  
<kbd> git clone </kbd> copies a remote repository to create a local repository with a remote called `origin` automatically set up.

### Step x:  go to working directory (your local terminal)

### Step x:  add remote

<kbd> git remote add origin <url> </kbd>
>my example

#### Step xb:  look at remotes
<kbd> git remote -v </kbd>

### Step 3:  update a repo
* copies changes from a remote repository to a local repository.
**Note:**  this is a good step to practice even though the first time you clone a repo it will already be up to date.  
syntax:  <kbd> git pull </kbd> 

 
### Step 4:  create a working branch
syntax:  <kbd> git branch <branch_name> </kbd>
>my example  
`git branch reshama_wip`

### Step 5:  switch to working branch
<kbd> git checkout <branch_name> </kbd>  
>my example  
`git checkout reshama_wip`

### Step 5:  create a file
* create a folder with your name here:  https://github.com/WiMLDS/python_advanced/tree/master/submissions
* `cd` into this folder, create a Python file with your name.  (Example:  `reshama.py`)

### Step 6:  add/stage a file:  `git add filename`
syntax:  `git add <file_name>`
>my example  
`git add reshama.py`

### Step 7:  commit a file:  `git commit -m 'adding my python name file`
syntax:  `git commit -m 'message'`  
>my example
 `git commit -m 'adding my python name file`
 
### Step 8:  push changes to your 'working branch':  `git push` 
syntax:  `git push origin <branch_wip>`  
>my example
`git push origin reshama_wip`


### Step x:  submit pull request (on GitHub)
