# git

 1. **初始化本地仓库：**

    bashCopy code

    `git init`

    这将在当前目录创建一个新的 Git 仓库。

 2. **添加远程仓库：**

    bashCopy code

    `git remote add origin <远程仓库URL>`

    这会将远程仓库添加到你的本地仓库的远程配置中。

    1. 上面两步可以合并为 `git clone url`

    2. 可以用`git remote -v`查看版本

    3. 删除本地Git 配置中删除了对远程仓库的引用`git remote remove origin`

 3. **创建并切换到新分支：**

    bashCopy code

    `git checkout -b <新分支名称>`

    这会创建并切换到一个新的本地分支。

 4. **添加你的代码：** 将你的代码添加到新分支上。

 5. **提交代码：**

    bashCopy code

    `git add . git commit -m "你的提交消息"`

    这会将你的代码提交到新分支上。

 6. **推送到远程仓库：**

    bashCopy code

    `git push origin <新分支名称>`

    这样，你的新分支及其代码就被推送到远程仓库中了。

 7. git branch 查看本地分支

 8. git reflog 查看本地的操作

 9. 删除分支之前最好commit，这样可以恢复

    1. git reflog查看哈希值

    2. 创建一个新的分支，指向该哈希值git checkout -b recover hash_value

10. 删除分支 

    1. `git branch -d name` (safely)

    2. `git branch -D name` (force)

请确保 `<远程仓库URL>` 是指向你想要推送的远程仓库的正确 URL。这样，你就能够在不克隆整个仓库的情况下创建一个新分支并将代码推送到远程仓库。