# manjaro-settings
manjaro linux セッテイング備忘録

# Caps キー　→　Ctrl
.bashrcに以下を追記
/usr/bin/setxkbmap -option "ctrl:nocaps"

# 日本語入力パッケージインストール(fcitx-mozc)
```
$ sudo pacman -S fcitx-mozc fcitx-gtk2 fcitx-gtk3 fcitx-qt5
```

## .xprofileを作成して以下を入力
```
export LANG="ja_JP.UTF-8"
export XMODIFIERS="@im=fcitx"
export XMODIFIER="@im=fcitx"
export GTK_IM_MODULE=fcitx
export QT_IM_MODULE=fcitx
export DefaultIMModule=fcitx
```

## .bashrcに以下を追記
```
export GTK_IM_MODULE=fcitx
export XMODIFIERS=@im=fcitx
export QT_IM_MODULE=fcitx
```

# gitプロンプト表示変更
https://qiita.com/varmil/items/9b0aeafa85975474e9b6

# runstant カーソルずれ問題対応
AURリポジトリから**monaco**フォントをインストール
パッケージ名：**ttf-monaco**

>参考記事
[manjaroでのchromeでprogateを含むブラウザ上のエディタのカーソルの位置がおかしくなる](https://qiita.com/kawadumax/items/8bbbc042c6f17407847e)
