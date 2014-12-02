# Gitコマンド勉強会 第5回 branch

## ブランチを表示してみる

### ローカルブランチを表示

```
$ git branch
```

### リモートブランチを表示

```
$ git branch -r
```

### 全てのブランチを表示

```
$ git branch -a
```

## ブランチを作成してみる

** 作成 **

```
$ git branch TEST-BRANCH
```

** 確認 **

```
$ git branch
```

** リモートにないことを確認 **

```
$ git branch -r
```

## リモートに push してみる

```
$ git checkout TEST-BRANCH
$ git push origin TEST-BRANCH
```

** リモートにあることを確認 **

```
$ git branch -r
```

** ブランチ内のファイルに変更を加えて違いを見てみる **

```
$ echo "branch-testです" > ./branch-test.txt
$ git add .
$ git commit -m 'test commit'
$ git push
```

https://github.com/flame1980/git-study

## ブランチを削除してみる

### ローカルブランチを削除してみる

```
$ git branch -d TEST-BRANCH
```

** ローカルブランチがないことを確認 **

```
$ git branch
```

### リモートブランチを削除してみる

```
$ git push origin :TEST-BRANCH
```

** リモートにないことを確認 **

```
$ git branch -r
```

** 全てでもみてみる **

```
$ git branch -a
```
