# Workflow to a Pull Request


[Step 1:  fork the repo](#section-1)  
[Step 2:  clone the repo](#section-2)  
[Step 3:  add an `upstream` remote](#section-3)  
[Step 4:  create a working branch](#section-4)  
[Step 5:  switch to working branch](#section-5)  
[Step 6:  create a file](#section-6)  
[Step 7:  start tracking the file](#section-7)  
[Step 8:  log the change](#section-8)  
[Step 9:  finalize the change:  `push`](#section-9)  
[Step 10:  On GitHub, submit a pull request (green button)](#section-10)

### <a name="section-1"></a>Step 1:  fork the repo
https://github.com/WiMLDS/python_advanced

### <a name="section-2"></a>Step 2:  clone the repo
syntax:  
`git clone <url>`  
>example:  
`git clone https://github.com/reshamas/python_advanced.git`


### <a name="section-3"></a>Step 3:  add an `upstream` remote
syntax:  
`git remote add upstream <original url>`  
>example:  
`git remote add upstream https://github.com/WiMLDS/python_advanced.git`


### <a name="section-4"></a>Step 4:  create a working branch
syntax:  
`git branch <new_branch_name>`    
>example:  
`git branch reshama_wip`

### <a name="section-5"></a>Step 5:  switch to working branch
syntax:  
`git checkout <branch_name>`
>example:  
`git checkout reshama_wip`

### <a name="section-6"></a>Step 6:  create a file
- create a folder with your name here:  `/Users/reshamashaikh/git_work/python_advanced/submissions`
- `cd` into this folder, create a folder with your name
    >example:  `/reshama/`
- create a Python file with your name
    >example:  `reshama.py`

### <a name="section-7"></a>Step 7:  start tracking the file
syntax:  
`git add <file_name>`
>example:  
`git add reshama.py`

### <a name="section-8"></a>Step 8:  log the change 
syntax:  
`git commit -m 'message`
>example:  
`git commit -m 'adding my python name file'`

### <a name="section-9"></a>Step 9:  finalize the change:  `push` 
`push` changes to your 'working branch'  
syntax:  
`git push <remote_name> <branch_name>`  
>example:  
`git push origin reshama_wip`

### <a name="section-10"></a>Step 10:  On GitHub, submit a pull request (green button)
