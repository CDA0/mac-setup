# Install via zsh

Install [`zsh-nvm`](https://github.com/lukechilds/zsh-nvm) and run `nvm upgrade`to upgrade.

# Install [Node.js](http://nodejs.org/) with [nvm](https://github.com/creationix/nvm) \(Node Version Manager\):

#### Install nvm

```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.1/install.sh | bash
```

#### Install nodejs

```
$ source ~/.bashrc # sources your bashrc to add nvm to path
$ command -v nvm  # check the nvm use message
$ nvm install node  # install most recent nodejs stable version
$ nvm ls  # list installed node version
$ nvm use node  # use stable as current version
$ nvm ls-remote  # list all the node versions you can install
$ nvm alias default node  # set the installed stable version as the default node 
```

## Npm usage

To install a package:

```
$ npm install <package> # Install locally
$ npm install -g <package> # Install globally
```

To install a package and save it in your project's `package.json` file:

```
$ npm install <package> --save
```

To see what's installed:

```
$ npm list # Local
$ npm list -g # Global
```

To find outdated packages \(locally or globally\):

```
$ npm outdated [-g]
```

To upgrade all or a particular package:

```
$ npm update [<package>]
```

To uninstall a package:

```
$ npm uninstall <package>
```



