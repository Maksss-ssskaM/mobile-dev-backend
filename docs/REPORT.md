### 1 task
![img.png](img/1.png)

cd .git
nano DESCRIPTION aboba

![img.png](img/1_2.png)
### 2 task
```
git cherry -v master 
git rebase -i HEAD~2
git rebase master
git merge ci
git branch -d ci
```
![img.png](img/2.png)

### 3 task
```
git log --reflog
git branch old-master 18eabfefb2ba8d1f5a87817ac36edb3b86e1335c
```
![img.png](img/3.png)

### 4 task
```
git blame prisma/seed.ts
```
![img.png](img/4.png)

### 5 task
```
git bisect start
npm run test
git bisect good/bad
```
![img.png](img/5.png)

### 6 task
```
git filter-branch --index-filter 'git rm --cached .env --ignore-unmatch' --prune-empty --tag-name-filter cat -- --all
```
![img.png](img/6_1.png)
![img.png](img/6_2.png)

### 7 task
```
git filter-branch --commit-filter '
    if [ "$GIT_AUTHOR_EMAIL" = "bakasaru@list.ru" ];
    then
            GIT_AUTHOR_NAME="AnnemariaRe";
            GIT_AUTHOR_EMAIL="annemariarepenko@gmail.com";
            git commit-tree "$@";
    else
            git commit-tree "$@";
    fi' HEAD
```
![img.png](img/7.png)

### 8 task
```
git config --global rerere.enabled true
git rerere diff
git merge feature
```
![img.png](img/8.png)

### 9 task
```
git fsck --lost-found
```
![img.png](img/9.png)

### 10 task
```
git gc
```
![img.png](img/10.png)

### 11 task
```
git commit -m "message"
```