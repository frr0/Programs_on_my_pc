# Programs on my pc

**Fedora**
```
sudo dnf install neovim python node texlive fzf ranger gcc zsh git onedrive valgrind pandoc firefox telegram-desktop thunderbird xournalpp vlc zathura
sudo dnf copr enable atim/lazygit -y
sudo dnf install lazygit
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
sudo rpmkeys --import https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/-/raw/master/pub.gpg 
printf "[gitlab.com_paulcarroty_vscodium_repo]\nname=gitlab.com_paulcarroty_vscodium_repo\nbaseurl=https://paulcarroty.gitlab.io/vscodium-deb-rpm-repo/rpms/\nenabled=1\ngpgcheck=1\nrepo_gpgcheck=1\ngpgkey=https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/-/raw/master/pub.gpg" |sudo tee -a /etc/yum.repos.d/vscodium.repo
sudo dnf install codium
sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
sudo dnf install obs-studio
```

## CLI programs

- Neovim
- Python3
- LazyGit
- Node.js
- Texlive
- Pdftex
- Fzf
- Ranger
- Gcc
- Java
- Zsh
- Ohmyzsh
- Git
- Onedrive
- [Dropbox](https://www.dropbox.com/install-linux)
- Valgrind
- pandoc


## GUI programs

- Firefox
- [Telegram](https://desktop.telegram.org/)
- Thunderbird
- Xournalpp
- VLC
- OBS
- KDE Connect
- Codium
- Zathura

