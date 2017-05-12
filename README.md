![](https://raw.githubusercontent.com/4-S/4S/master/_img/4s-wide.png)

### The simplest package manager for aliases.

# Install 4S

### Install on FreeBSD - .cshrc edition

```
cd ~ ; mkdir .4s-core ; fetch https://raw.githubusercontent.com/4-S/4S/master/csh/.4s-index ; echo 'source ~/.4s-index' >> ~/.cshrc ; cd ~/.4s-core ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/csh/.4s-core/.4s-core-index ; cd ~ ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/csh/.4s-core-custom-updater-config ; source ~/.cshrc
```
Paste that into a Terminal.

### Install on Ubuntu - .bashrc edition
```
cd ~ ; mkdir .4s-core ; wget -q https://raw.githubusercontent.com/4-S/4S/master/bash/.4s-index -O .4s-index ; echo 'source ~/.4s-index' >> ~/.bashrc ; cd ~/.4s-core ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/bash/.4s-core/.4s-core-index -O .4s-core-index ; cd ~ ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/bash/.4s-core-custom-updater-config -O .4s-core-custom-updater-config ; source ~/.bashrc
```
Paste that into a Terminal.

![](https://raw.githubusercontent.com/4-S/4S/master/_img/4-install.gif)


# What Does 4S Do?

1. 4S makes managing and updating alias files _simple_ and _easy_.
1. 4S makes installing and configuring services with secure defaults easy, with _simple_ shortcuts.
1. 4S reduces complex multi-step tasks into _single word shortcuts_.
1. 4S takes a _fraction of the time_ it takes to do by hand.
1. 4S is a _sane and human readable_ alias.

4S installs additional Core aliases inside its own folder.

```
user@host:~$ ls -a
.
..
.4s-core/
.4s-core-custom-updater-config
.4s-index
.bashrc
```

Trivially create and add your own alias files. An alias can be as simple as a shortcut to a series commands.
Example:

```
alias mytest='date ; uname -a ; sudo apt update'
```

## Community Discussion
Text and voice chat on the public mumble server.
**Join the Public Mumble**
Server: `pub.bringyourwallet.com`
Port: `64738`
