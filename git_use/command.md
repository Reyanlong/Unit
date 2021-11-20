```
git status    // 查看状态

git add      // 添加追踪

git rm --cached    // 移除追踪

git commit    // 提交


/** 查看日志 */
git log --pretty=online
git log --online
git reflog

git reset --hard 哈希值       // 版本改变

git reset --hard HEAD  // 恢复到当前指针的版本

git stash  // 存入暂存区

git stash pop     // 恢复之前缓存的工作版本


linux命令    tail -n 3 filename     // 显示最后几行


git diff   // 比较不同，没有参数与暂存区比较

git diff HEAD^^^ filename   // 与HEAD之前的第三个版本比较
git diff HEAD~数字 filename     //与HEAD之前的第<参数数字>版本比较

```


```
git branch -v    // 查看分支

git branch    // 创建分支

git checkout 分支名    // 切换分支


/** 先要切换回（要合并到的那个分支去） 合并分支 */
git merge
 /** 出现冲突 就要手动审核 */
git add filename
git commit -m "日志信息"    // 不带文件名
/** 完成合并 */



git remote -v     // 地址别名查看

/** 创建仓库代号  origin是自己起的别名 仓库地址为http地址 或者ssh地址 */
git remote add origin 仓库地址


git push origin master  // 将当前本地仓库推送到远程库


/** git pull 等于 git fetch 加 git merge */


/** 其它有用的命令 */
git cherry --pick
git rebase


/** 设置当前用户信息 */
git config --global user.name 用户名
git config --global user.email 邮件

git config user.name 用户名
git config user.email 邮件


````