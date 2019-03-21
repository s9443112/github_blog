# Git
# Base oprating way

![ALT_Text](https://s9443112.github.io/github_blog/2019/2019-01-12/IMG_2798.JPG)


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

git remote

```
$ git remote add <name> <url>
$ git remote remove <name>
$ git remote
```



If there's any problem, please try to use git help

* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
