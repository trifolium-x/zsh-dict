## zsh-dict 介绍

zsh-dict 是使用 zsh 脚本编写的一个命令行翻译工具，使用百度翻译接口。

fork 自 [whinc/dict工程](https://github.com/whinc/dict) 经过修改

## 安装

复制下面命令到终端中执行即可：(假设安装在~/zsh/zsh-dict中)

1. 从仓库克隆

   ```shell
   git clone https://github.com/trifolium-wang/zsh-dict.git ~/.zsh/zsh-dict
   ```

2. 添加到你的. `~/.zshrc` 文件中

   ``` shell
   source ~/.zsh/zsh-dict/zsh-dict.zsh
   ```

3. 启动一个新的终端session

## 在oh-my-zsh中安装

1. 从仓库clone

   ```shell
   git clone https://github.com/trifolium-wang/zsh-dict.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-dict
   ```

2. 将插件添加到 Oh My Zsh 的插件列表中以加载（在 `~/.zshrc` 中）：

   ```shell
   plugins=( 
       # other plugins...
       zsh-dict
   )
   ```

3. 启动一个新的终端session

## dict 使用

用法：`dict [word]...`
说明：如果只有一个单词，则翻译该单词。如果有超过一个单词，则视作句子进行翻译。

```shell
$ dict hello
你好

$ dict hello world
你好世界
```
## 不维护了
