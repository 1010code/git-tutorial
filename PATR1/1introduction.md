# intro

Git是一個分佈式版本控制系統（DISTRIBUTED VERSION CONTROL SYSTEM:DVCS）

Git 是被一位 Linus Torvalds 的工程師所開發的，在他工作時用開發 Linux 系統

## 如何使用
- command line interface
- GUI tools

鍵入 git help 會列出所有 Git 指令
```
git help
```

初始設定
```
$ git config --global user.name "Gregg Pollack"
$ git config --global user.email gregg@codeschool.com
$ git config --global color.ui true
```

`git init` 會初始化你本機下的專案路徑並儲存於 `.git` 檔案中檔案中
```
git init
```

`git status` 會檢查你專案中未被上版控的檔案有哪些(untrack)
```
git status
```
## Add file to staging area
若要追蹤這些檔案就要把這些檔案新增到狀態區(staging area)
```
git add 檔案名稱
git add .
git add --all
```

## Commit changes

```
$ git commit -m "Create a README."
```
## GIT TIMELINE HISTORY
查詢 commit 的紀錄
```
git log
```
