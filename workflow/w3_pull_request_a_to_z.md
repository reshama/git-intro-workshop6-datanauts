# Workflow:  Submit Pull Request, Steps A to Z

## Step 1:  fork the repo (on GitHub)
https://github.com/WiMLDS/python_advanced

## Step 2:  copy forked url for cloning 
<img src="images/github_clone_button.png" align="left" height="40" width="180" >    
Click on the green button for your forked GitHub repo, and ensure it is showing the url for "Clone with HTTPS"  (other option is "Clone with SSH").  Copy that URL.    


  
    
    
>my example  
```text
https://github.com/reshamas/python_advanced.git
```

## Step 3:  go to working directory (your local terminal)
Go to your working directory  
>my example
```bash
cd /Users/reshamashaikh/ds/gitsample
```

## Step 4:  clone the repo  
<kbd> git clone <url> </kbd> 
>my example
```bash
git clone https://github.com/reshamas/python_advanced.git
```

## Step 4:  `cd` into the repo
<kbd> cd <repo_name> </kbd>
>my example
```bash
cd python_advanced 
```

## Step 5:  look at remotes
<kbd> git remote -v </kbd>
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
```

## Step 6:  add 'upstream' remote
<kbd> git remote add upstream <url> </kbd>
>my example
```bash
git remote add upstream https://github.com/WiMLDS/python_advanced.git
```

## Step 7:  look at remotes
<kbd> git remote -v </kbd>  
>my example
```bash
origin	https://github.com/reshamas/python_advanced.git (fetch)
origin	https://github.com/reshamas/python_advanced.git (push)
upstream	https://github.com/WiMLDS/python_advanced.git (fetch)
upstream	https://github.com/WiMLDS/python_advanced.git (push)
```

## Step 8:  update a repo
This step copies changes from a remote repository to a local repository.  
**Note:**  this is a good step to practice even though the first time you clone a repo it will already be up to date.   

<kbd> git pull </kbd> 

 
## Step 9:  create a working branch
<kbd> git branch <branch_name> </kbd>
>my example  
`git branch reshama_wip`

## Step 10:  switch to working branch
<kbd> git checkout <branch_name> </kbd>  
>my example  
`git checkout reshama_wip`

## Step 11:  create a file
Note:  We will submit a pull request to the repo and that file will go here:  https://github.com/WiMLDS/python_advanced/tree/master/submissions  

- create a folder in the repo with your name here:  `python_advanced/submissions`
- `cd` into this folder, create a folder with your name
- create a Python file (Example:  `test_python_file.py`)

<kbd> pwd </kbd>  
<kbd> ls </kbd>  
<kbd> cd submissions </kbd>  
<kbd> mkdir reshama </kbd>  
<kbd>  cd reshama </kbd>  
<kbd>  touch test_python_file.py </kbd>  

>my example
```bash
% pwd
/Users/reshamashaikh/ds/gitsample/python_advanced
% ls
total 24
-rw-r--r--  1    66 Nov 22 07:31 README.md
-rw-r--r--  1   506 Nov 22 07:31 q1_define_structures.md
-rw-r--r--  1   328 Nov 22 07:31 q2_function.md
drwxr-xr-x  6   204 Nov 22 07:31 submissions
% cd submissions 
% mkdir reshama
% cd reshama
% touch test_python_file.py
% ls
total 0
-rw-r--r--  1   0 Nov 22 09:06 test_python_file.py
% 
```
    
## Step 12:  add/stage a file
<kbd> git add <file_name> </kbd>  
>my example  
`git add test_python_file.py`

## Step 13:  commit a file
<kbd> git commit -m 'message' </kbd>
>my example
 `git commit -m 'adding my python test file`
 
## Step 14:  push changes to your 'working branch'
<kbd> git push origin <branch_wip> </kbd>  
>my example
`git push origin reshama_wip`


## Step 15:  submit pull request (on GitHub)

