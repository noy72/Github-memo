# Github/Gitの操作メモ
## ブランチ
```
git branch
```
ブランチを一覧表示
```
git checkout -b <branch name>
```
ブランチの作成，切り替え
```
git merge --no-ff <branch name>
```
現在のブランチに，branch nameをマージする．
コンフリクトしたら，編集してadd-\>commit．
```
git log --graph
```
ブランチを図で表示
```
git push -u origin <branch name>
```
ブランチをリモートリポジトリに追加する
```
git checkout -b <branch name> <branch name in remote repo>
```
リモートのブランチをチェックアウトする

## コミットの変更
```
git reset --hard <commit id>
```
ローカルリポジトリを指定されたコミット後の状態に戻す．
```
git commit --amend
```
コミットメッセージの修正
```
git rebase -i HEAD~<number>
```
最新コミットからnumberまでのコミットを対象として，コミットを変更する．

## 検索
```
http://<repo url>/compare
```
ブランチ間の差分を見る
