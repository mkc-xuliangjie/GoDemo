## this is a git command tutorial

### 1.repository  仓储

* client repository :  HEAD

* remote repository : origin

### 2.branch 分支

#### 2.1 创建一个名称为branch1的分支

* git branch branch1  

#### 2.2 切换到branch1分支

* git checkout branch1

### 3.commit  一次新的提交

### 4.githash   会产生对应的一次唯一的提交标示

#### 相关命令：

* git status

* git diff

* git add

* git commit -a -m

* git push

### 5.代码的回滚:

#### 回滚到指定的commit，显示变更的文件

* git reset  githash   

#### 回滚到指定的commit ,不显示变更的文件

* git reset --hard  githash   

#### 如果需要回滚到指定的commit并且提交的话：

##### 先针对这个分支做备份

* git branch branch1BackUp  

##### 回滚到指定的commit ,不显示变更的文件

* git reset --hard  githash   
 
##### 强制覆盖remote端代码

* git push -f  

### 6.tag

#### 标签，可以为某一个具体的commit打一个标记, 为以后可能会对当前版本做比较或者启用做记录

#### 创建tag

* git tag -a v1.0.1 36e0061849ec7ceeaf55f3a22ee3d49d7ad08aaa  -m 'add tag for current commit'

* git push origin v1.0.1

#### 删除tag

* git tag -d tagname 

### 7.merge  代码的合并

#### 将指定的githash合并到当前的branch

* git merge githash

#### 查看当前branch的log

* git log