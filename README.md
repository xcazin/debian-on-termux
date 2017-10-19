# debian-on-termux

what is it:

- a shell script to install Debian 9 (stretch) via debootstrap in a termux-app environment

how to use it:

- install termux-app 
- download 'debian_on_termux.sh' from this repository to termux home directory '/data/data/com.termux/files/home'
```
    cd
    wget https://raw.githubusercontent.com/sp4rkie/debian-on-termux/master/debian_on_termux.sh
```
- set perms and execute the script
```
    chmod 755 debian_on_termux.sh
    ./debian_on_termux.sh
```
- watch the installation process by
```
    tail -F $HOME/deboot_debian9/debootstrap/debootstrap.log
```
- if all went well a script is created in $HOME/bin. To enter the debian guest system just type
```
    $HOME/bin/enter_deb
```
- in case of a problem just drop me an email:-)

reference:
    [How to install Debian 9.2 chroot termux? #1645](https://github.com/termux/termux-packages/issues/1645#issuecomment-337564650)
