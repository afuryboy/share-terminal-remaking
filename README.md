# share-terminal-remaking
iterm2+oh-my-zsh 终端小改造:blush:

why:1、不好看 2、bash不显示git分支 3、终端中无法用编辑器打开文件。

want：
iterm2快速呼出

![](http://img.cnsecer.com/wp-content/uploads/2015/06/8ad0ba005f155dfb3b0aa5c299148b2a.jpg)

各种主题

![](https://cloud.githubusercontent.com/assets/2618447/6316862/70f58fb6-ba03-11e4-82c9-c083bf9a6574.png)
![](https://cloud.githubusercontent.com/assets/2618447/6316861/70f3c4ce-ba03-11e4-88a5-0b423dd5a2ce.png)

[iterm2传送门](http://www.iterm2.com/)

[oh-my-zsh传送门](http://ohmyz.sh/)

安装完毕之后

mac默认的shell是bash,所以需要改为zsh
```sh
cd /
chsh -s /bin/zsh
```

然后

```sh
cd ~
ls -a
```
一堆文件忽略，我们只需要关注 .zshrc .oh-my-zsh

```sh
nano .zshrc
```
ZSH_THEME="robbyrussell"  //默认主题

ZSH_THEME="ys"

如果想查看oh-my-zsh的主题
```sh
cd .oh-my-zsh
cd themes
ls
```
列出所有可用主题



如果我们想在终端中用编辑器打开文件只需在.zshrc文件末尾加下面一段代码

alias atom='/Applications/Atom.app/Contents/MacOS/Atom'

alias subl='/Applications/SublimeText.app/Contents/SharedSupport/bin/subl'

alias code='/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin/code'

使用：
```sh
atom 文件名
subl 文件名
code 文件名
```

iterm2快速呼出配置:
preferences  keys
![](http://img.cnsecer.com/wp-content/uploads/2015/06/ec145771a8c5cda82698d419983920f0.png)

至此应该就能达到want效果。
