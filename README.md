![](https://raw.githubusercontent.com/4-S/4S/master/_img/4s-wide.png)

### The simplest package manager for aliases.

[![Join the chat at https://gitter.im/4_S/Lobby](https://badges.gitter.im/4_S/Lobby.svg)](https://gitter.im/4_S/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# What Does 4S Do?

1. 4S makes managing and updating alias files _simple_ and _easy_.
1. 4S makes installing and configuring services with secure defaults easy, with _simple_ shortcuts.
1. 4S reduces complex multi-step tasks into _single word shortcuts_.
1. 4S takes a _fraction of the time_ it takes to do by hand.
1. 4S is a _sane and human readable_ alias.

4S installs additional Core aliases inside its own folder.

# Install 4S

## FreeBSD - .cshrc edition

### Instructions

Get dependencies and change your current shell.

`pkg install signify ca_root_nss ; echo $0 ; chsh -s /bin/csh ; echo $0`

### Install

```
cd ~ ; mkdir .4s-core ; cd ~/.4s-core ; fetch https://raw.githubusercontent.com/4-S/4S/master/freebsd-csh/.4s-index ; echo 'source ~/.4s-core/.4s-index' >> ~/.cshrc ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/freebsd-csh/.4s-core/.4s-core-index ; cd ~ ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/freebsd-csh/.4s-core-custom-updater-config ; source ~/.cshrc
```
Paste that into a Terminal.

## Ubuntu - .bashrc edition

### Instructions

_Linux instructions are a temporarily a little messy._

Get dependencies `brew`+`minisign`. `linuxbrew-wrapper` has problems, install with this method:

```
sudo apt install ruby git curl build-essential python-setuptools wget ; ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install)" ; echo 'export PATH="/home/linuxbrew/.linuxbrew/bin:$PATH"' >> ~/.bashrc ; echo 'export MANPATH="/home/linuxbrew/.linuxbrew/share/man:$MANPATH"' >> ~/.bashrc ; echo 'export INFOPATH="/home/linuxbrew/.linuxbrew/share/info:$INFOPATH"' >> ~/.bashrc ; echo 'export XDG_DATA_DIRS="/home/linuxbrew/.linuxbrew/share:$XDG_DATA_DIRS"' >> ~/.bashrc ; PATH="/home/linuxbrew/.linuxbrew/bin:$PATH" ; brew update --force ; brew install bash-completion ; echo "  [ -f /home/linuxbrew/.linuxbrew/bash_completion ] && . /home/linuxbrew/.linuxbrew/etc/bash_completion" >> ~/.bashrc ; source ~/.bashrc ; brew install minisign
```

![](https://raw.githubusercontent.com/4-S/4S/master/_img/4s-install-ubuntu.gif)

### Install

```
cd ~ ; mkdir .4s-core ; wget -q https://raw.githubusercontent.com/4-S/4S/master/ubuntu-bash/.4s-index -O ~/.4s-core/.4s-index ; echo 'source ~/.4s-core/.4s-index' >> ~/.bashrc ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/ubuntu-bash/.4s-core/.4s-core-index -O ~/.4s-core/.4s-core-index ; cd ~ ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/ubuntu-bash/.4s-core-custom-updater-config -O ~/.4s-core-custom-updater-config ; source ~/.bashrc
```
Paste that into a Terminal.


## macOS - .bash_profile edition

### Instructions

Get dependencies.

[`brew`](https://brew.sh/) and `brew install minisign`

![](https://raw.githubusercontent.com/4-S/4S/master/_img/4s-install-mac.gif)

### Install

```
cd ~ ; mkdir .4s-core ; curl -L https://raw.githubusercontent.com/4-S/4S/master/macos-bash/.4s-index -o ~/.4s-core/.4s-index ; echo 'source ~/.4s-core/.4s-index' >> ~/.bash_profile ; curl -L https://raw.githubusercontent.com/4-S/4S-core/master/macos-bash/.4s-core/.4s-core-index -o ~/.4s-core/.4s-core-index ; curl -L https://raw.githubusercontent.com/4-S/4S-core/master/macos-bash/.4s-core-custom-updater-config -o ~/.4s-core-custom-updater-config ; source ~/.bash_profile
```
Paste that into a Terminal.

# Load Your Custom Aliases

Trivially create and add your own alias files. An alias can be as simple as a shortcut to a series commands.
Example:

```
alias mytest='date ; uname -a ; sudo apt update'
```

### [Learn More](https://github.com/4-S/4S-custom)


# Top Supporters

Monthly supporters only.

Amount     | Supporter Name            | Supporter Domain       
-----------|---------------------------|------------------------
$50/month  | [Tugger Hosting][thgh]    | [tuggerhosting.com][th]
$50/month  | [Yella Dog Networks][ydn] | [yelladognetworks.com][ydn]

[reelsense]: https://github.com/reelsense
[byw]: http://frothymix.info
[thgh]: https://github.com/TuggerHosting
[th]: https://tuggerhosting.com/
[ydn]: https://yelladognetworks.com


## Support 4S Development

### **[Support Now](https://reelsense.tv/donate)**

**Support 4S development** and maintenance and get simple tutorials & aliases designed for your Cloud VPS!: _Vultr_, _DreamHost_, _Digital Ocean_, _Amazon EC2_, or _Google Cloud Platform_.

Help simplify the Cloud VPS customer experience.
> Create a Mumble server in 50 seconds on Vultr for $2.50/month!


## Community Discussion

Text and voice chat on the public mumble server.

**Join the Public Mumble**

Server: `pub.bringyourwallet.com`

Port: `64738`
