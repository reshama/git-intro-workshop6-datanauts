# Workflow 1:  Create and Update My Repo

## Step 1:  create a repo (on GitHub)
- Click on `+` next to your profile picture
- Select `New Repository`
- Repository name:  `gitclass`
- Description (optional):  `test project for git`
- `Public` repos are free
- Check box for `Initialize this repository with a README` :white_check_mark: :heavy_exclamation_mark:
- Select green button `Create repository`

## Step 2:  copy URL for cloning

Click on the green button for your forked GitHub repo, and ensure it is showing the url for **Clone with HTTPS**  (other option is "Clone with SSH").  Copy that URL.    <br> 
<img src="../images/github_clone_button.png" align="left" height="40" width="180" >   <br> <br>
    
>my example  
```text
https://github.com/reshamas/gitclass.git
```

## Step 3:  go to working directory (your local terminal)
Go to your working directory  
>my example
```bash
cd /Users/reshamashaikh/ds/gitsample
pwd
/Users/reshamashaikh/ds/gitsample
```  

## Step 4:  clone the repo  
<kbd> git clone <url> </kbd> 
>my example
```bash
git clone https://github.com/reshamas/gitclass.git
Cloning into 'gitclass'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
```

## Step 5:  `cd` into the repo
<kbd> cd <repo_name> </kbd>
>my example
```bash
cd gitclass 
```

## Step 6:  look at remotes
<kbd> git remote -v </kbd>
>my example
```bash
git remote -v
origin	https://github.com/reshamas/gitclass.git (fetch)
origin	https://github.com/reshamas/gitclass.git (push)
```

## Step 7:  update a repo
This step copies changes from a remote repository to a local repository.  
**Note:**  this is a good step to practice even though the first time you clone a repo it will already be up to date.   

<kbd> git pull </kbd> 

## Step 8:  list branches
<kbd> git branch </kbd>  
>my example
```git
git branch
* master
```
 
## Step 9:  create a working branch
<kbd> git branch <branch_name> </kbd>
>my example  
`git branch reshama_wip`

## Step 10:  list branches
<kbd> git branch </kbd>  
>my example
```git
git branch
* master
  reshama_wip
```

## Step 11:  switch to working branch
<kbd> git checkout <branch_name> </kbd>  
>my example  
`git checkout reshama_wip`


## Step 12:  create a file
<kbd>  ls </kbd>  
<kbd> touch mercury.md </kbd>  

>my example
```bash
ls
touch mercury.md
```
```bash
ls
total 8
-rw-r--r--  1   32 Nov 22 09:39 README.md
% touch mercury.md
% ls
total 8
-rw-r--r--  1   32 Nov 22 09:39 README.md
-rw-r--r--  1    0 Nov 22 09:49 mercury.md

	mercury.md
```
    
## Step 13:  add/stage a file
<kbd> git status </kbd>  
<kbd> git add <file_name> </kbd>   
	
>my example  
```bash
git status
git add mercury.md 
```
```bash
% git status
On branch reshama_wip
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	mercury.md
nothing added to commit but untracked files present (use "git add" to track)
% git add mercury.md 
```

## Step 14:  commit a file
<kbd> git status </kbd>   
<kbd> git commit -m 'message' </kbd>  
	
>my example
```bash
git status
git commit -m 'adding first planet'
```
	
```bash
% git status
On branch reshama_wip
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   mercury.md

% git commit -m 'adding first planet'
[reshama_wip 3950dd9] adding first planet
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 mercury.md
```


## Step 15:  push changes to your 'working branch'
<kbd> git status </kbd>  
<kbd> git push origin <branch_wip> </kbd>  
	
>my example
```bash
git push origin reshama_wip
```	

```bash
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 273 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/reshamas/gitclass.git
 * [new branch]      reshama_wip -> reshama_wip
 ```
 
## Step 16:  submit pull request (on GitHub)
Go to GitHub and refresh your browser.  
My url is:  https://github.com/reshamas/gitclass  

Select green button "Compare and pull request"  
<img src="../images/pull_request_button.png" align="left" height="40" width="180" >   <br> <br>

---

## Summary of Steps
<kbd> cd /Users/reshamashaikh/ds/gitsample </kbd>  
<kbd>  pwd </kbd>   
<kbd> git clone https://github.com/reshamas/gitclass.git </kbd>   
<kbd> cd gitclass </kbd>   
<kbd> git remote -v </kbd>  
<kbd> git pull </kbd>  
<kbd> git branch </kbd> <kbd> git branch reshama_wip </kbd>  
<kbd> git branch </kbd> <kbd> git checkout reshama_wip </kbd>  
<kbd>  ls </kbd>  
<kbd> touch mercury.md </kbd>  
<kbd>  ls </kbd>  
<kbd>  git status </kbd> <kbd>  git add mercury.md </kbd>  		  
<kbd>  git status </kbd> <kbd>  git commit -m 'adding first planet' </kbd>  		  
<kbd>  git status </kbd> <kbd>  git push origin reshama_wip </kbd>  

