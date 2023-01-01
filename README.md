# Terminal Profile

My terminal profile.

## Installation

### Powershell

1. Install [Powershell](https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D), [Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701) & [NerdFonts](https://www.nerdfonts.com/).
2. Install [Scoop](https://scoop.sh/).
   ```
   iwr -useb get.scoop.sh | iex
   scoop install curl sudo jq
   ```
3. Install [oh-my-posh](https://ohmyposh.dev/).
   ```
   Install-Module posh-git -Scope CurrentUser -Force
   Install-Module oh-my-posh -Scope CurrentUser -Force
   ```
4. Install [Terminal-Icons](https://github.com/devblackops/Terminal-Icons).
   ```
   Install-Module -Name Terminal-Icons -Repository PSGallery -Force
   ```
5. Install [PSReadline](https://github.com/PowerShell/PSReadLine).
   ```
   Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
   ```
6. Install [fzf](https://github.com/junegunn/fzf) & [PSFzf](https://github.com/kelleyma49/PSFzf).
   ```
   scoop install fzf
   Install-Module -Name PSFzf -Scope CurrentUser -Force
   ```
7. Copy _default.omp.json_ to _%homepath%/.config/powershell_.
8. Add lines in _powershell/user_profile.ps1_ to the Powershell profile.

### Ubuntu

1. Install [NerdFonts](https://www.nerdfonts.com/).
2. Install [oh-my-posh](https://ohmyposh.dev/).
   ```
   sudo wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/posh-linux-amd64 -O /usr/local/bin/oh-my-posh
   sudo chmod +x /usr/local/bin/oh-my-posh
   ```
3. Install [logo-ls](https://github.com/Yash-Handa/logo-ls).
   ```
   wget -q https://github.com/Yash-Handa/logo-ls/releases/download/v1.3.7/logo-ls_Linux_x86_64.tar.gz
   tar zxvf logo-ls_Linux_x86_64.tar.gz
   cd logo-ls_Linux_x86_64/
   sudo install -v logo-ls /usr/local/bin/
   sudo cp logo-ls.1.gz /usr/share/man/man1/
   ```
4. Install [Ble.sh](https://github.com/akinomyoga/ble.sh).
   ```
   git clone --recursive https://github.com/akinomyoga/ble.sh.git
   make -C ble.sh install PREFIX=~/.local
   echo 'source ~/.local/share/blesh/ble.sh' >> ~/.bashrc
   ```
5. Install [fzf](https://github.com/junegunn/fzf).
   ```
   git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
   ~/.fzf/install
   ```
6. Copy _default.omp.json_ to _~/.poshthemes_.
7. Add or change lines in _ubuntu/.bashrc_ to the _~/.bashrc_ file.