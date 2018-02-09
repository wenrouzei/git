# git
git操作命令

## 1. 克隆仓库
git clone git@github.com:wenrouzei/git.git
## 管理分支
## 2. 查看分支
### 2.1 查看本地分支
使用 git branch命令，如下：

'$ git branch`

`* master`

`* develop`

*标识的是你当前所在的分支。

### 2.2 查看远程分支
命令如下：

>git branch -r

### 2.3 查看所有分支
命令如下：

>git branch -a

### 2.4 本地创建新的分支
命令如下：

>git branch [branch name]

例如：

>git branch gh-dev

### 2.5 切换到新的分支
命令如下：

>git checkout [branch name]

例如：

```$ git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.
```

### 2.6 创建+切换分支
创建分支的同时切换到该分支上，命令如下：

>git checkout -b [branch name]

`git checkout -b [branch name]` 的效果相当于以下两步操作：

>git branch [branch name]
>git checkout [branch name]


### 2.7 将新分支推送到github
命令如下：

>git push origin [branch name]

例如：

>git push origin gh-dev

### 2.8 删除本地分支
命令如下：

>git branch -d [branch name]

例如：

>git branch -d fix-bug

### 2.9 删除github远程分支
命令如下：

>git push origin :[branch name]

分支名前的冒号代表删除。 
例如：

>git push origin :fix-bug
