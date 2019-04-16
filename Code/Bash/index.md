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
```
* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
