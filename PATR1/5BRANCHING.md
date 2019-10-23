# BRANCHING

## 把分支 push 到 GitHub
```
git push origin 分支
```

## 查看遠端分支
```
git branch -r
```

## Remote show
顯示雲端分支
```
git remote show origin
```
## 刪除 Remote 分支
```
git push origin :分支
```
必須刪除本地分支
```
git branch -D 分支
```
## 若發現遠端分支被刪
```
git remote prune origin
```

# Tag
發布版本時
## 新增一個tag
```
git tag -a v0.0.1 -m 'vsrsion 0.0.1'
```

## 上傳
```
git push --tags
```
## 進入 tag
```
git checkout v0.0.1
```



