# Upgrade

```
sudo dnf update
sudo dnf upgrade
```

# Upgrade to the newest version
```
sudo dnf -y update
sudo dnf install dnf-plugin-system-upgrade
sudo dnf system-upgrade download –releasever=INSERT NUMBER
sudo dnf system-upgrade reboot
```

# Install and Remove apps

## DNF

### Install
```
sudo dnf install i3
```
### Remove
```
sudo dnf remove i3
```
## RPM

### Install

```
sudo rpm -i sample_file.rpm

sudo dnf localinstall sample_file.rpm
```
### Remove

```
sudo rpm -e sample_file.rpm

sudo rpm -qpR sample_file.rpm
```

The system should list all the dependencies:

    -q – This option tells RPM to query the file
    -p – This option lets you specify the target package to query
    -R – This lists the requirements for the package

## Tar

```
tar -zxvf eclipse-inst-jre-linux64.tar.gz && cd eclipse-installer && ./eclipse-inst
```

## Copr

### Install
```
 sudo dnf copr enable eddsalkield/swaylock-effects 
sudo dnf install swaylock-effects
```

### Remove

```
sudo dnf copr disable kwizart/fedy  
```

# Shell

```
cat /etc/shells
chsh -s /path
```

# Git ssh keys 
```
ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub
```
> Then select and copy the contents of the id_ed25519.pub file
> displayed in the terminal to your clipboard  
> settings/ssh keys  
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent  
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account

## git .gitignore update

```
git rm -r --cached .
git add -A
git commit -am 'Removing ignored files'
```

# Graphic tablet

```
xsetwacom list
```
<!--number can change-->
```
xsetwacom set 15 MapToOutput HDMI-1  
```

# Audio problems

https://askubuntu.com/questions/75828/external-microphone-not-working
```
pavucontrol
hdajackretask
alsa-tools-gui
```

# Programs

<!--name of programs-->
```
xprop
```

## i3wm Setting commands

Graphic tablet
```
xsetwacom set 21 MapToOutput eDP-1
xsetwacom list devices
```

## wifi
```
iw dev
nmtui
```

## bluetooth
```
bluetoothctl
$ power on
$ agent on
$ scan on
Only the first time
$ pair AA:BB:CC:DD:EE:FF
$ connect AA:BB:CC:DD:EE:FF
# scan off when you found your device
scan off
exit
```

## Screen
```
xrand
r --output DP-1 --mode 1280x1024
xrandr
```

## zip

```
zip -9 -e -r -q name folder_to_be_zipped/
unzip folder.zip
```

## dir to file
```
tar czf myfiles.tar.gz mydirectory/    
```

## file to dir
```
tar xzf myfiles.tar.gz
```

## enc
```
gpg -e -r myname myfiles.tar.gz
```

## dec
```
gpg -d myfiles.tar.gz.gpg
```



## BETTER encr
```
gpgtar --encrypt --output <out_file_name> -r <recipient> <dir_name>
```

## dec
```
gpgtar --decrypt <out_file_name>
```

# gdb

<!--## debug-->

## inside vim

```
file program
b 1
b Main.c:1

r f1.txt fn.txt
```

```
define a
n
info locals
end
```

```
p i
display i
```

## terminal 

```
gdb ./program

b 1
b Main.c:1

r f1.txt fn.txt

define a
n
l
info locals
end

p i
display i
```

## terminal with ui

```
gdb -tui ./program

b 1
b Main.c:1
rb program.c:.

r f1.txt fn.txt

record
rc rn

c n

define a
n
info locals
end

p i
display i
```
