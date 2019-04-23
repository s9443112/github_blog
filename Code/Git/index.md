# Git
# Base oprating way

![ALT_Text](2019/2019-01-12/IMG_2798.JPG)

## 基本 commit 流程

先做基本的commit 流程

```
$ git add .
```
```
$ git commit -m "DB FIX"
```
然後要跟群組上的做合併
```
$ git pull luhao master
```

假設有衝突的話 COMFLICT  
使用VSCODE解完衝突後  
在下一次commit
```
$  git add .
```
```
$  git commit -m "fix comflict"
```
都做完完成後 就可以推上自己的Repo

```
$ git push origin dev
```
然後在送MR給群組 自己merge (github 是PR)

## Git remote

```
$ git remote add <name> <url>
$ git remote remove <name>
$ git remote
```

Git branch

## Git 復原hard模式 reset commit

先觀看所有git紀錄
```
$ git log --oneline
e12d8ef (HEAD -> master) add database.yml in config folder
85e7e30 add hello
657fce7 add container
abb4f43 update index page
cef6e40 create index page
cc797cd init commit
```

git reset指令倒退兩步
```
$ git reset HEAD~2 --hard
```

不僅 Commit 看起來不見了，檔案也消失了。接著可使用 reflog 指令來看一下紀錄：
```
$ git reflog
657fce7 (HEAD -> master) HEAD@{0}: reset: moving to HEAD~2
e12d8ef (origin/master, origin/HEAD, cat) HEAD@{1}: checkout: moving from cat to master
e12d8ef (origin/master, origin/HEAD, cat) HEAD@{2}: checkout: moving from master to cat
```

可以把剛剛 hard reset 的東西再次撿回來了。
```
$ git reset e12d8ef --hard
```



此指令保留所有git指令紀錄
```
$ git reflog
```





If there's any problem, please try to use git help

* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
