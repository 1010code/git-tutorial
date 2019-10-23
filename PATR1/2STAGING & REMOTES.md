# STAGING & REMOTES

在修改檔案中你忘己你在這支檔案修改了什麼可以下以下指令來觀看內容
```
git diff
```


若要看 stage 的檔案有修改什麼下這個指令
```
git diff --staged
```

##  UNSTAGING FILES
把在 stage 的檔案變回 untrack 未追蹤， HEAD 代表最後一次 commit 也就是目前的分支
```
git reset HEAD 檔案名稱
```

##  DISCARD CHANGES

把這個檔案設定不要追蹤，放棄更變
```
git checkout -- LICENSE
```

## 快速 add 和 commit
 SKIP STAGING AND COMMIT

```
git commit -a -m "Modify readme"
```

##  UNDOING A COMMIT 跟上一次重新提交
不小心忘記提交某檔，會結合上一次的重新提交一次
Undo last commit, put changes into staging
```
git reset --soft HEAD^
```
hard 會整個拋棄並重新提交(原本檔案刪除)
## Change the last commit
重新修改提交訊息
```
git commit --amend -m '重新寫提交訊息'
```

##  PUSHING TO REMOTE
- origin
  - remote repository name
- master
  - local branch to push
```
git push -u origin master
```

## 從遠端數據庫下載更新
同步遠端數據庫的資料同步到本機
```
git pull
```

### WORKING WITH REMOTES
- To add new remotes
```
git remote add <name> <address>
```
- To remove remotes
```
git remote rm <name>
```
- To push to remotes
```
git push -u <name> <branch> 通常是 master
```

## 這些指令pull後不能使用
```
git reset --soft HEAD^  
git commit --amend -m "New Message"
git reset --hard HEAD^ 
git reset --hard HEAD^^
```
