## Main branch merge to local branch
```bash
git fetch origin
git rebase origin/master
```

不停重复下面的命令
```bash
git rebase —continue
```

手动merge conflict

```bash
git add .
```

直到没有问题了

```bash
git pull
git push
```

处理merge conflict

最后git status检查一下

然后给master发一个pull request


## Branch switch
```bash
git checkout -b ${branch_name} origin/${branch_name}
```

## Useful links

http://rogerdudler.github.io/git-guide/
[https://github.com/521xueweihan/git-tips](https://github.com/521xueweihan/git-tips)