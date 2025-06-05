# ZSH configuration
This is my personal zsh configuration. It contains a few definitions I like and a highly customized command prompt that displays any git branch encountered but also shows any available and activated python virtual environments.

If you want a generic highly customizable zsh configuration environment than I can recommend [Oh My Zsh](https://ohmyz.sh)


To use this you best clone this (or fork it and clone your own fork) to your home directory in a directory called .zsh
```
git clone https://github.com/eniese/zsh.git ~/.zsh
```

To properly initialize some environment variables create a file: ~/.zshenv
```
ZENV="$HOME/.zsh/env"
ZFUNC="$HOME/.zsh/functions"
fpath=( "$ZFUNC" "${fpath[@]}" )
autoload "$ZFUNC"/*
... add anything you want ...
```

Now you can start using elements from this configuration in your:  ~/.zshrc:
```
source_once colors
source_once unicode
source_once prompts
PROMPT="$PROMPT3"
```


