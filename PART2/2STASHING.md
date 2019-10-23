# STASHING
將你的紀錄暫存丟入stack
- WIP (work in progress)
```
git stash save //後面亦可加訊息說明
git stash apply  //回放回來
git stash pop  //彈出來並移除
git stash list  //查詢stack list
git stash list -stat // 可觀看修改記錄
git stash show stash@{1} //觀看指定修改紀錄
git stash apply stash@{1} //指定回放哪個
git stash drop //移除彈出最上
git stash clear //一次刪除所有暫存
```
## 若 stash 衝突時
若stash要重新修改暫存先pop再
```
git stash save --keep-index //保持原來位置
```

