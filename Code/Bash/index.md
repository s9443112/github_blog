# Bash
# Base oprating way


基本登入
```
$ ssh root@127.0.0.1
```

遠端下載
```
$ scp root@192.168.0.102:/home/1.txt /home/download
```

服務管理
```
$ systemctl start OOXX
$ systemctl restart OOXX
$ systemctl stop OOXX
$ systemctl enable OOXX
$ systemctl disable OOXX
$ systemctl status OOXX
```

測試網路
```
$ ping www.google.com
```

Command history 
```
$ history 
$ history -c  ## Delete all history
$ history -d 1010  ## Delete number 1010 of history

## 使用fish shell

依照作業系統指令安裝fish (Ubuntu)
```
$ apt install fish 
```
  使用fish 作為你的預設shell
  所有的shell都條列在 /etc/shells 檔裡面:
    bin/bash
/bin/csh
/bin/ksh
/bin/sh
/bin/tcsh
/bin/zsh
/usr/local/bin/fish # 新增你的 fish 在這裡

使用chsh 改變你的預設shell
```
$ chsh -s /usr/local/bin/fish
```



```
* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
