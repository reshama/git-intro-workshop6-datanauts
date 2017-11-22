# Clone a Repository
---
**Q:  What is cloning?**  
**A:  Making a copy of something.**

![orphan black](images/orphan_black.jpg)

---

## Select green button "Clone or download" and copy url

### Go to directory on local computer  
For me, it is: 
`/Users/reshamashaikh/git_work`  

>my example
```bash
~/git_work  master ✗                                                                  ◒  
▶ pwd
/Users/reshamashaikh/git_work
```

#### Clone repo
`git clone https://github.com/reshamas/starting_git.git`  

>my example  
```bash
~/git_work  master ✗                                                                  ◒  
▶ git clone https://github.com/reshamas/starting_git.git
Cloning into 'starting_git'...
remote: Counting objects: 15, done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 15 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (15/15), done.
Checking connectivity... done.
```

### `cd` into cloned repo

```bash
▶ pwd
/Users/reshamashaikh/git_work/starting_git

▶ ls
total 0
drwxr-xr-x  7   238 Nov 14 11:29 data-science-from-scratch
drwxr-xr-x  6   204 Nov 14 11:48 starting_git

~/git_work  master ✗                                                                  ◒  
▶ cd starting_git 

~/git_work/starting_git  master ✔                                                    6m  
▶ 
```
## Check out the remote
**Remotes** are copies of a repo on another computer **(or on a service like Github)**  

**Example:**  
* `upstream` [organization repo]
* `origin`   [your forked repo]

**Note:**  
* notice you have push and pull access  

>my example  
```bash
▶ git remote -v
origin	https://github.com/reshamas/starting_git.git (fetch)
origin	https://github.com/reshamas/starting_git.git (push)
```

### We can 'pull' updates from GitHub version
```bash
▶ git pull
Already up-to-date.
```

## Make changes on local computer 

### Let's make a change on local computer and push changes up to GitHub
Use an editor of your choice to create a python file which will print your name.  
My file `print_name.py` contains the following line of code:  
```python
print("My name is Reshama")
```

```bash
~/git_work/starting_git  master ✔                                                   11m  
▶ emacs print_name.py

~/git_work/starting_git  master ✗                                                 11m ◒  
▶ python print_name.py 
Hello, my name is Reshama

~/git_work/starting_git  master ✗                                                 12m ◒  
▶ 
```

## We made a change!  How does git track it? `git status`
To see what changes have been made since last `git pull`, type `git status`  
```bash
▶ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	print_name.py

nothing added to commit but untracked files present (use "git add" to track)

~/git_work/starting_git  master ✗                                                 14m ◒  
▶ 
```
---

## Next up:  how do we send those changes up to GitHub? :boom:


