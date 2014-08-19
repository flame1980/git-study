# 実践

## git stash

### stash に退避してみる

```
$ vi test01.txt
$ cat test01.txt
$ git stash save
$ cat test01.txt
```

### stash から取得してみる

```
$ git stash apply
$ cat test01.txt
```

### stash の一覧を見てみる

```
$ git stash list
```

### stash から削除してみる

```
$ git stash drop
```

### commit と組み合わせて試してみる

```
$ vi test02.txt
$ cat test02.txt
$ git commit -m 'stash のテストコミット'
$ git stash
$ cat test02.txt
$ git stash apply
$ cat test02.txt
```

### 複数stash

```
$ vi test03.txt
$ cat test03.txt
$ git stash
$ cat test03.txt
$ vi test03.txt
$ cat test03.txt
$ git stash
$ cat test03.txt
$ git stash list
$ git stash apply stash@{0}
$ cat test03.txt
$ git stash apply stash@{1}
$ cat test03.txt
$ git stash drop stash@{0}
$ git stash list
$ git stash drop stash@{0}
$ git stash list
```

