[toc]

### 概念

#### 集中式与分布式

|          |              分布式              |                       集中式                       |
| :------: | :------------------------------: | :------------------------------------------------: |
| 代码存储 | 每个人的电脑上就有一份完整的代码 |             只有中心服务器拥有一份代码             |
|  安全性  |                无                | 有安全性问题，当中心服务器挂了所有人都没办法工作了 |
|   连网   |            不需要连网            |                  需要连网才能工作                  |
|   效率   | 新建分支、合并分支操作速度非常快 |         新建一个分支相当于复制一份完整代码         |
|   实例   |               Git                |                        SVN                         |

#### SSH传输设置

Git 仓库和 Github 中心仓库之间的传输是通过 SSH 加密

创建SSH Key

```
 ssh-keygen -t rsa -C "youremail@example.com"
```





### 创建新的 git 仓库：git init

### 克隆远端服务器上仓库：git clone username@host:/path/to/repository

### 工作流：

- 工作目录：持有实际文件
- 暂存区：缓存区域，临时保存改动

- HEAD：指向最后一次提交结果

### 添加和提交：git add \<filename>、git add *、git commit -m "代码提交信息"

### 推送改动:git push origin master

### 仓库连接到某个远程服务器:git remote add origin \<server>

### 创建新的分支：git checkout -b new_branch

### 切换回主分支：git checkout master

### 删除分支：git branch -d new_branch

### 将分支推送到远端仓库：git push origin\<branch>

### 更新本地仓库:git pull

### 合并其他分支到当前分支:git merge --no-ff  \<branch>

### 操作失误替换本地改动而不影响已经提交到暂存区的内容：git checkout -- \<filename>

### 放弃本地改动与提交，恢复至服务器最新：git fetch origin、git reset --hard origin/master

