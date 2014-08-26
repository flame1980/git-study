# 実践

## git status

### 通常

```
$ git status
```

### 簡易表示

```
$ git status -s
```

### 未定義ファイルの扱い

```
$ git status -u
$ git status -uno
$ git status -unormal
$ git status -uall
```

## git log

### 通常

```
$ git log
```

### ホワイトスペース無視

```
$ git log -w
```

### 件数指定

```
$ git log -n 3
$ git log -2
```

### コミット者指定

```
$ git log --author=sakai
$ git log --author=hoge
```

### 期間指定

```
$ git log --since=2014-08-24
$ git log --until=2014-08-24
$ git log --since=2014-08-20 --until=2014-08-21
```
