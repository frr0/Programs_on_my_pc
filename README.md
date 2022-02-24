# Programs on my pc

**Fedora**
```
sudo dnf install i3 neovim python node texlive fzf ranger gcc zsh git onedrive valgrind pandoc firefox telegram-desktop thunderbird xournalpp vlc zathura polybar rofi sway waybar wlr-randr brightnessctl swaylock pavucontrol
sudo dnf copr enable atim/lazygit -y
sudo dnf install lazygit
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
sudo rpmkeys --import https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/-/raw/master/pub.gpg 
printf "[gitlab.com_paulcarroty_vscodium_repo]\nname=gitlab.com_paulcarroty_vscodium_repo\nbaseurl=https://paulcarroty.gitlab.io/vscodium-deb-rpm-repo/rpms/\nenabled=1\ngpgcheck=1\nrepo_gpgcheck=1\ngpgkey=https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/-/raw/master/pub.gpg" |sudo tee -a /etc/yum.repos.d/vscodium.repo
sudo dnf install codium
sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
sudo dnf install obs-studio
```
```
CNTX={users|orgs}; NAME={username|orgname}; PAGE=1
curl "https://api.github.com/$CNTX/$NAME/repos?page=$PAGE&per_page=100" |
  grep -e 'git_url*' |
  cut -d \" -f 4 |
  xargs -L1 git clone
```
   - Set `CNTX`=users and `NAME`=yourusername, to download all your repositories.
   - Set `CNTX`=orgs and `NAME`=yourorgname, to download all repositories of your organization.


## CLI programs

- i3wm
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
- polybar
- sway
- waybar
- rofi
- herbe
- wlr-randr
- brightnessctl
- swaylock
- pavucontrol


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

