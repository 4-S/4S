![](https://raw.githubusercontent.com/4-S/4S/master/_img/4s-wide.png)
# Install 4S

### 4S - FreeBSD .cshrc edition

```
cd ~ ; mkdir .4s-core ; fetch https://raw.githubusercontent.com/4-S/4S/master/csh/.4s-index ; echo 'source ~/.4s-index' >> ~/.cshrc ; cd ~/.4s-core ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/csh/.4s-core/.4s-core-index ; cd ~ ; fetch https://raw.githubusercontent.com/4-S/4S-core/master/csh/.4s-core-custom-updater-config ; source ~/.cshrc
```
Paste that into a Terminal.

### 4S - Ubuntu .bashrc edition
```
cd ~ ; mkdir .4s-core ; wget -q https://raw.githubusercontent.com/4-S/4S/master/bash/.4s-index -O .4s-index ; echo 'source ~/.4s-index' >> ~/.bashrc ; cd ~/.4s-core ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/bash/.4s-core/.4s-core-index -O .4s-core-index ; cd ~ ; wget -q https://raw.githubusercontent.com/4-S/4S-core/master/bash/.4s-core-custom-updater-config -O .4s-core-custom-updater-config ; source ~/.bashrc
```
Paste that into a Terminal.


# What Does 4S Do?

1. 4S is a sane and human readable alias.
1. 4S installs and configures services, with secure and simple defaults.
1. 4S does this in a fraction of the time it takes to do by hand.
