---
layout: post
title: "Setting up git workspace on Linux or Mac"
date: 2018-07-09 24:07:20 +0530
description: A tutorial about setting up git workspace on linux
img: # Add image post (optional)
tags: [Tutorial, Git, Linux] # add tag
---

#### First of all downloading necessary files

* Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash) in your home directory with the name `git-completion.bash`.
* Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh) in your home directory with the name `git-prompt.sh`.
* Download `bash_profile_course` [here](https://www.udacity.com/api/nodes/3341718587/supplemental_media/bash-profile-course/download?_ga=1.37232743.672083044.1467344711).
* If you already have a file in your home directory named `.bash_profile`, copy the content from `bash_profile_course` and paste it at the bottom of `.bash_profile`. Otherwise, move `bash_profile_course` to your home directory and rename it to `.bash_profile`. If you use Linux, you may need to name this file `.bashrc` instead of `.bash_profile`. (If you're curious to learn more about how bash prompts work, [see this page](http://www.cyberciti.biz/tips/howto-linux-unix-bash-shell-setup-prompt.html).)

#### Make sure you can start your editor from the terminal

If you use Sublime, you can do this by add the following line to your `.bash_profile` (you may need to change the path if Sublime is installed in a different location for you):

```
alias subl="/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl"
```

#### Making Git configurations

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Sublime, or if Sublime is installed in another location for you. See [this page](https://help.github.com/articles/associating-text-editors-with-git/) for the correct command for a couple of other popular text editors. For any other editor, you'll need to enter the command you use to launch that editor from the terminal.

```shell
$ git config --global core.editor "'/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl' -n -w"
$ git config --global push.default upstream
$ git config --global merge.conflictstyle diff3
```


#### Restart the terminal
You'll need to close and re-open the terminal before all your changes take effect.<br>
Link to [GitHub Gist](https://gist.github.com/akashgiricse/744ef21fc8a81f24e1230feb7af4e3e5)<br>
Source [Udacity](https://classroom.udacity.com/courses/ud775)