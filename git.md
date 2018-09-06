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
   git pull
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



### log

```
git log %ファイル名%
```



