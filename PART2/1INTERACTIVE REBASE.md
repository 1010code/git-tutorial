# INTERACTIVE REBASE
若開啟分支時 master 有新提交紀錄可以移植過來目前分支，融合
```
git rebase master
```

交換
```
git rebase -i HEAD~2
```
pitch 改 reword 可以修改訊息

##  SPLIT COMMITS
拆開commit

先使用edit 在reset
```
edit b3f1649 Add unicorn
git reset HEAD^
git rebase --continue  
```

## squash
回去修改內容
```
squash b3f1649 Add unicorn
```
