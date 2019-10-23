# HISTORY AND CONFIGURATION

先前所介紹的`git log`可以得知所有提交訊息、SHA hash、作者、時間，缺點難以閱讀

##  COLORIZING THE LOG

```
git config --global color.ui true
git log --pretty=oneline  //只顯示一行
git log --oneline -p //包含修改記錄
git log --oneline --stat //＋-文件一覽
git log --oneline --graph //顯示圖流程
```

##  DATE RANGES

```  
$ git log --until=1.minute.ago
until
 
$ git log --since=1.day.ago
since (days)
 
$ git log --since=1.hour.ago
since (hours)
 
$ git log --since=1.month.ago --until=2.weeks.ago
since & until (relative)
 
$ git log --since=2000-01-01 --until=2012-12-21
since & until (absolute)
```

##  EARLIER COMMITS
可觀看這幾次提交變動什麼
```
 $ git diff HEAD^   //parent of latest 
 $ git diff HEAD^^
 $ git diff HEAD~5  //commit five commits ago
 git diff master elephant // 察看兩分之不同
```
也可以用 SHAs 搜尋

## Blame
此指令可以看單一檔案的修改記錄

```
git blame 檔案 --date short
```
 
## 刪除檔案
```
git rm 檔案
```

##  UNTRACKING FILES
取消追蹤檔案
$ git rm --cached development.log
