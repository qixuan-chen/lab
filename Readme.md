## update website guide 

### clone the repository


first, 

if

```{zsh}
# the default repository name will be origin 
git clone https://github.com/qixuan-chen/lab.git
```

if 

```{zsh}
# cd to the root directory
```

### make some preliminary check


```{zsh}
# check what are included in the directory
ls
# check git status 
git status
# check remote repository
git remote -v
# check branch
git branch
```

if

```{zsh}
git add .
git commit -m "Update website"
git pull origin main
git push origin main
```

if 

```{zsh}
# This command will delete any local changes that have not been committed yet
git fetch origin
git reset --hard origin/main
```

### modify the content you want

if 

```{zsh}
hugo server -D
```

then open the website with adress, When you finish, run following code.

```{zsh}
hugo serve
```

```{zsh}
git status
git add .
git commit -m "describe the modification"
git push 
```