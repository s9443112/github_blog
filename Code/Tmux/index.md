# Tmux
# Base oprating way

## New session

New session
```
$ tmux new -s doghow -n doghow 
```

## 在 Tmux 視窗下的 Vim 失去顏色

  在一般情況下vim自訂的顏色能正常顯示
  但是在tmux視窗下的vim失去顏色
  所以如果要tmux支持256 colors
```
$ tmux -2
```

如果不想那麼麻煩，就設定在.bashrc
```
alias tmux='tmux -2'
```

## 本地有tmux 遠端也有tmux 下如何操作

  通常我們在操作tmux時，我們會按快捷鍵Ctrl+b
  但如果我們遠端在別台linux上，同時那台機器也有tmux
  那如果只按 "一次 " Ctrl+b ，會操作到我們電腦上的tmux
  但如果我們按 "兩次" Ctrl+b 我們就可以操作遠端上的tmux 

* * *

# Like Button

<iframe class="lc-margin-top-64 lc-margin-bottom-32 lc-mobile" data-v-b66e9a5a="" frameborder="0" src="https://button.like.co/in/embed/s9443112/button"> </iframe>

* * *

{% if site.disqus.shortname %}
  {% include disqus_comments.html %}
{% endif %}
