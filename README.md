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
```
git branch -m <new branch name>
```
ブランチをリネームする

## コミットの変更
```
git reset --hard <commit id>
```
ローカルリポジトリを指定されたコミット後の状態に戻す．
```
git commit --amend
```
コミット上書き．コミットメッセージの修正
```
git rebase -i HEAD~<number>
```
最新コミットからnumberまでのコミットを対象として，コミットを変更する．

## 検索
```
http://<repo url>/compare
```
ブランチ間の差分を見る

## Pull request
1. Fork
1. Clone
1. Branchの作成
トピックブランチで作業する
1. リモートブランチの作成
ローカルのトピックブランチに対応するブランチを作る

