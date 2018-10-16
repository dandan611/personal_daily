# personal_daily

## Table of Contents



---

### Microsoft on Linux の設定
http://www.atmarkit.co.jp/ait/articles/1608/08/news039.html
⇒ひとまず置いておく。Vagrantで環境構築ができたらこっちに乗り換えてみる

### Cygwinのviコマンドで方向キーを入力するとABCDと出た場合

```
$ vi ~/.exrc
set nocompatible
set backspace=indent,eol,start
```

https://qiita.com/MT-01/items/510236860fd511ecec70

### Cygwin のプロンプトに Git のブランチを表示する

```
$ wget https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh
$ mv git-prompt.sh /etc/profile.d/
```

以下を`.bashrc`に追記

```
source /etc/profile.d/git-prompt.sh
export PS1='\u@\h \w$(__git_ps1)\n\$ '
```

https://qiita.com/amano41/items/5d2aed152a16f9d884df

以上。

