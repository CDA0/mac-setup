# Zsh

We'll install `zsh` for all the features offered by `oh-my-zsh`. The installation and usage is really intutive. The `env.sh` is a config file we maintain so as to not pollute the `~/.zshrc` too much. `env.sh` holds aliases, exports, path changes etc.

### Zsh

Install zsh and zsh completions using homebrew

```
$ brew install zsh zsh-completions
$ chsh -s /usr/local/bin/zsh
```

If there is a message about using a non standard shell you need to add the shell to `/etc/shells`

```
$  sudo -s
$  echo /usr/local/bin/zsh >> /etc/shells
$  exit
```

The above `chsh` command will now work.

Now you can customise your shell using Antigen.

#### Antigen

```
$ curl https://cdn.rawgit.com/zsh-users/antigen/v1.4.0/bin/antigen.zsh > ~/.antigen.zsh
```

I host my dot files on github so you can get my ~/.zshrc from there.

