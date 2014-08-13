# 実践

## git clone

### 普通にクローンしてみる

```
git clone https://github.com/flame1980/git-study.git
```

### ブランチを指定してクローンしてみる

```
git clone -b develop https://github.com/flame1980/git-study.git
```

### クローンするディレクトリを指定する

```
git clone https://github.com/flame1980/git-study.git test-source
```

## 流れに沿ってやってみる

まずはファイルを準備
```
$ touch test03.txt
$ vi test03.txt
```

git 操作
```
$ git pull
$ git add test03.txt
$ git commit -m test03.txt
$ git push
```
