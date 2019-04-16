# Vim
# Base oprating way

安裝Vim (依作業系統指令 本實例參照ubuntu)
```
$ apt install vim 
``` 

## 安裝樣式以及基本功能

基本上我是參照我朋友的Github上寫好的樣式來套用
使用reimu-vim 
[https://github.com/m85091081/reimu-vim](https://github.com/m85091081/reimu-vim/)
```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/m85091081/reimu-vim/master/loader.sh)"
```

### 安裝教學問題
如果ycmd安裝失敗的話

```
$ cd /root/.vim/plugged/YouCompleteMe
$ git pull
$ ./install.py
$ python3 ./install.py --clang-completer
```

提示 "CMAKE_CXX_COMPILER-NOTFOUND "

  Check for working CXX compiler: CMAKE_CXX_COMPILER-NOTFOUND 
  CMake Error: your CXX compiler: "CMAKE_CXX_COMPILER-NOTFOUND" was not found.
  Please set CMAKE_CXX_COMPILER to a valid compiler path or name.

解决方法：
```
$ sudo apt-get install g++
```


* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
