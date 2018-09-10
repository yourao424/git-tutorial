# GitHubの使い方

## Gitの準備

```
git init
```

または

```
git clone %gitのURL%
```



## Gitでの作業

### GitHubから引っ張ってくる場合

1. 作業場所を最新の状態にする

   ```
   git pull origin master
   ```

2. ブランチを作成する

   ```
   git branch %branch名%
   ```

3. 作成したブランチに切り替える

   ```
   git checkout %ブランチ名%
   ```

   または

   ```
   git checkout -b %ブランチ名%
   ```

4. ソースコードを修正する

5. 修正したファイルをブランチに追加する

   ```
   git add %ファイル名%
   ```

   または

   ```
   git add .
   ```

6. コミットする

   ```
   git commit
   ```

7. リモートホストへの反映させる

   ```
   git push origin %ブランチ名%
   ```



### 1から作る場合

4. から



## Gitコマンドの基本操作

### branch

```
ローカルブランチの一覧を見る
git branch

リモートブランチの一覧を見る
git branch --remote

ブランチの作成
git branch %ブランチ名%

ブランチの削除
git branch --delete %ブランチ名%
※マージの海にかかわらず削除したい場合は -D
```



### checkout

```

ブランチの切り替え
git checkout %ブランチ名%

作業場所で修正したファイルを元に戻す
git checkout -- %ファイル名%

ファイルを以前のコミットに戻す
git checkout %リビジョン% %ファイル名%

```



### commit

```
コミット
git commit

直前のコミットを修正する
git commit --amend 
```



### log

```
git log %ファイル名%
```



### merge

```groovy
git merge %ブランチ名%

例：AにBの変更を適用する
git checkout A

git merge B
```



### rebase

```
git rebase %ブランチ名%

%ブランチ名%に現在のブランチで行ったすべてのコミットを適用する
```



### diff

```
作業場所で変更した内容を確認する
git diff
```



### revert

```
git revert
```



### reset 

```
git reset
```



### cherry-pick

```
気が向いたら追記
```



### .gitignore

```
Gitの管理に含めないファイルを指定するためのファイル
```



## 補足説明

pull =  fetch + merge origin/master

