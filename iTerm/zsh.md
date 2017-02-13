# Zsh

We'll install `zsh` for all the features offered by `oh-my-zsh`. The installation and usage is really intutive. The `env.sh` is a config file we maintain so as to not pollute the `~/.zshrc` too much. `env.sh` holds aliases, exports, path changes etc.

### Zsh

Install zsh and zsh completions using homebrew

```
    brew install zsh zsh-completions
```

Now you can customize your shell using two frameworks Prezto or Oh My Zsh. So follow one of the two sections below.

#### Antigen

```
curl https://cdn.rawgit.com/zsh-users/antigen/v1.4.0/bin/antigen.zsh > antigen.zsh
```

#### 

### env.sh

```
    #!/bin/zsh

    # PATH
    export PATH="/usr/local/share/python:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    export EDITOR='subl -w'
    # export PYTHONPATH=$PYTHONPATH
    # export MANPATH="/usr/local/man:$MANPATH"

    # Virtual Environment
    export WORKON_HOME=$HOME/.virtualenvs
    export PROJECT_HOME=$HOME/Projects
    source /usr/local/bin/virtualenvwrapper.sh

    # Owner
    export USER_NAME="YOUR NAME"
    eval "$(rbenv init -)"

    # FileSearch
    function f() { find . -iname "*$1*" ${@:2} }
    function r() { grep "$1" ${@:2} -R . }

    #mkdir and cd
    function mkcd() { mkdir -p "$@" && cd "$_"; }

    # Aliases
    alias cppcompile='c++ -std=c++11 -stdlib=libc++'

    # Use sublimetext for editing config files
    alias zshconfig="subl ~/.zshrc"
    alias envconfig="subl ~/Projects/config/env.sh"
```



