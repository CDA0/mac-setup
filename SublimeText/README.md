# Sublime Text

With the terminal, the text editor is a developer's most important tool. Everyone has their preferences, but unless you're a hardcore [Vim](http://en.wikipedia.org/wiki/Vim_\(text_editor\)\) user, a lot of people are going to tell you that [Sublime Text](http://www.sublimetext.com/) is currently the best one out there.

Install the latest version of Sublime Text with homebrew, you should also have a license handy to enter after this is installed.

```
brew tap versions
brew cask install sublime-text-dev
```

**Note**: At this point I'm going to create a shortcut on the OS X Dock for both for Sublime Text and iTerm. To do so, right-click on the running application and select **Options &gt; Keep in Dock**.

Sublime Text is not free, but it has an unlimited "evaluation period". Anyhow, we're going to be using it so much that even the seemingly expensive $60 price tag is worth every penny. If you can afford it, It is adviced that you [support](http://www.sublimetext.com/buy) this awesome tool. :\)

Let's create a shortcut so we can launch Sublime Text from the command-line:

```
$ ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

Now you can open a file with `$ subl myfile.py` or start a new project in the current directory with `$ subl .`. Pretty cool. We'll configure Sublime more in the next few sections.

Using Dropbox we can sync our settings for Sublime between computers.





