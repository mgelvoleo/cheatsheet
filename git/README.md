## Git Basic Command 

```
Command
git init
```


```
Command
git add file
```



```
Command
git commit -m "Commit here"
```

## Git display the info of branchs

```
Command
git ls-tree -r main
```

```
Command
git log --oneline
```

```
Command
git branch
```




NOTE: Before you push it to you repository you need to have the token for to used as password and dont forget the ssh key for your
machine you can check my youtube tutorial on how to create a secure ssh key.


```
Command
git remote add origin https://github.com/sample
```

```
Command
git push -u origin main 
```

## Config if the credential was setup  to check
```
Command
git config --list
```

```
Command
git config --global user.name "Mark Gelvoleo"
```


```
Command
git config --global user.email "sample@email.com"
```


## How to create a branch
```
Command
git branch developer1
```

```
Command
git checkout developer1
```


## How to merge the create branch to main

```
Note: You need to be point in the main to execute the command
Command
git merge developer1
```

## How to make an alias on git to make your life easier in coding
```
git config --global alias.br branch
git config --global alias.co commit
git config --global alias.st status
git config --global alias.list 'log --oneline'
```


